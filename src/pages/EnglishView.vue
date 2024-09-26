<script lang="ts" setup>
import { ref } from 'vue';
import { useRouter } from 'vue-router';


  const modalSkill = ref<boolean[]>([false, false]);
  const dialog = ref<boolean[]>([false, false, false, false, false]);
  const router = useRouter();

  // Função para abrir o modal específico
function openDialog(index: number) {
  dialog.value[index] = true;
}

// Função para fechar o modal específico
function closeDialog(index: number) {
  dialog.value[index] = false
}

function openSkill(index: number) {
  modalSkill.value[index] = true;
}

function closeSkill(index: number) {
  modalSkill.value[index] = false
}


  function portugues(){
    router.push('/');
  }
  </script>


<template>
  <v-app>
    <v-app-bar :elevation="3" class="nav">

  <v-app-bar-title class="nav-title">Gustavo Cortezia
     <v-btn @click="portugues" class="ml-4 btn-lingua"><img src="../assets/brasil_circulo.png" alt="" width="51px"></v-btn>
     <v-btn class="btn-lingua"><img src="../assets/USAworld_flags_6_-512.webp" alt="" width="33px"></v-btn>
    </v-app-bar-title>

<div class="nav-btns">
  <v-btn href="#about-me">About Me</v-btn>

  <v-btn href="#education">Education</v-btn>

  <v-btn href="#hard-skills">Hard Skills</v-btn>

  <v-btn href="#soft-skills">Soft Skills</v-btn>

  <v-btn href="#projects">Projects</v-btn>

  <v-btn href="#contacts">Contacts</v-btn>
</div>



</v-app-bar>

<div class="home-bg">
  <v-row class="mx-15">
    <v-col md="6" sm="12" class="col">
      <div class="img-div">
        <a href="https://www.linkedin.com/in/gustavocortezia/" target="_blank">
    <img class="minha-foto rounded-circle" width="400px" height="400px" src="../assets/Captura de tela 2024-07-15 144029.png" alt="My Photo">
  </a>
      </div>
    </v-col>

    <v-col md="6" sm="12" class="col">
      <div class="home-text-div d-flex">

        <h1 class="gustavo-nome mb-6">Gustavo Cortezia</h1>
        <div class="home-text-div">
          <p class="home-text" id="about-me"> Full Stack Web Developer | Computer Science | VueJS | Laravel | MySQL | PHP | JavaScript | TypeScript | Java | HTML | CSS</p>
        </div>
        </div>
    </v-col>
  </v-row>


</div>

<div class="about-div">
  <v-card class="about-card pa-15">

<v-card-title >
  <p class="about-card-title">
    About Me
  </p>
</v-card-title>

<v-card-text>
  <p class="about-card-text">
    I am currently in the fourth semester of Computer Science at the University of Vale do Rio dos Sinos (Unisinos) and finishing the 1000-hour Web Full Stack Development program at Growdev, a technology school that trains professionals for the job market. Through a selection process with over 1,200 candidates, I was selected by Sicredi Pioneira and received a full scholarship for the program. I completed all my primary and secondary education at Colégio Sinodal in São Leopoldo, recognized as one of the best schools in Rio Grande do Sul.
  </p>
</v-card-text>

<v-card-text>
  <p class="about-card-text">
    The technical training I have already acquired gives me the confidence to start a career as a full stack developer. I have solid knowledge in HTML, CSS, JavaScript, Java, PHP, Laravel, Bootstrap, TypeScript, VueJS, Vuetify, and MySQL. Some of my strengths include social skills, creativity, emotional intelligence, problem-solving, and advanced English. I am a very determined and committed person, always striving to learn and deliver my work with quality, helping to create a better future.
  </p>
</v-card-text>

</v-card>
</div>

<div class="educacao" id="education">
  <h1 class="education-title mt-15">My Education</h1>

  <v-row class="div-container" no-gutters>
    <v-col md="6" sm="12" class="col-educ">
      <v-card class="unisinos-card mx-auto" width="400" height="550">
        <v-img class="align-end text-white" height="300" width="400" src="../assets/image.png" cover></v-img>
        <div class="pa-5">
          <v-card-title class="educ-card-title">Unisinos University</v-card-title>
          <v-card-text>
            <h2>Computer Science</h2>
            <h3 class="mb-5"> (03/2023 - now)</h3>
            <v-btn class="btn-style" @click="openSkill(0)">Skills Developed</v-btn>
          </v-card-text>
        </div>
      </v-card>
    </v-col>

    <v-dialog
  class="dialog-unisinos"
    v-model="modalSkill[0]"
    width="auto"
  >
    <v-card class="modal-education pa-6" max-width="800">
    <v-btn
      class="btn-close-modal ms-auto"
      text="x"
      @click="closeSkill(0)"
    ></v-btn>
       <img class="unisinos_vista_img" src="../assets/unisinos_vista.png" alt="">
       <v-card-title class="modal-title ma-3 mb-15">Unisinos University</v-card-title>
       <h2 class="habilidades-titulo">Skills Developed:</h2>
       <h3 class="habilidades-desenvolvidas">Emotional Intelligence | Algorithms, Innovation | Agile Methodologies | Database | Software Engineering | Java</h3>
      </v-card>
    </v-dialog>

    <v-col md="6" sm="12" class="col-educ">
      <v-card class="unisinos-card mx-auto" width="400" height="550">
        <v-img class="align-end text-white" height="300" width="400" src="../assets/logosinodalquadrado.webp" cover></v-img>
        <div class="pa-5">
          <v-card-title class="educ-card-title">Sinodal School</v-card-title>
          <v-card-text>
            <h2>Basic Education</h2>
            <h3 class="mb-5">(2006 - 2022)</h3>
            <v-btn class="btn-style" @click="openSkill(1)">Skills Developed</v-btn>
          </v-card-text>
        </div>
      </v-card>
    </v-col>
  </v-row>
</div>

  <v-dialog
  class="dialog-unisinos"
    v-model="modalSkill[1]"
    width="auto"
  >
    <v-card class="modal-education pa-6" max-width="800">
    <v-btn
      class="btn-close-modal ms-auto"
      text="x"
      @click="closeSkill(1)"
    ></v-btn>
       <img class="unisinos_vista_img" src="../assets/sinodal_vista.png" alt="">
       <v-card-title class="modal-title ma-3 mb-15">Sinodal School</v-card-title>
       <h2 class="habilidades-titulo">Skills Developed:</h2>
       <h3 class="habilidades-desenvolvidas">Problem Solving | Creativity | Leadership | Communication | Teamwork</h3>
      </v-card>
    </v-dialog>



    <div class="grow-div mt-15">

<v-card
  class="grow-card mx-auto"
  width="1500px"
  height="450px"
>
  <v-img
    class="grow-img"
    height="450px"
    width="500px"
    src="../assets/growdev-logo-branco.png"
    cover
  ></v-img>
  <div class="grow-content">
    <h1 class="title-grow-card ma-5 mb-10">Starter Growdev Program - <span class="despertar-dev">Despertar.dev</span></h1>

    <h3>The Starter Full Stack Developer Program is a complete training that goes from programming and technology fundamentals to the development of a complete software with front-end, back-end, database, cache, ensuring quality with automated tests and deployment of the system in production. Additionally, students have the opportunity to apply their knowledge to projects contracted by companies, developed in Growdev's software factory.</h3>
<br>
  <h3>Fui selecionado pela<span class="despertar-dev"> Sicredi Pioneira</span>, por meio de um processo seletivo, para ganhar uma bolsa de estudos (100%) para o Starter Growdev Program, do qual me garantiu muito aprendizado e experiência </h3>
  <h3>Carga Horária: 1000 horas</h3>
  </div>


</v-card>

</div>


  <div class="conhecimentos-div" id="hard-skills">
  <h1 class="conhecimentos-title mb-15">Skills</h1>


  <div class="conhecimentos">

    <div class="skill-div" data-skill="HTML">
      <img class="skill" src="../assets/conhecimentos/html.png" alt="">
    </div>

    <div class="skill-div"  data-skill="CSS">
      <img class="skill" src="../assets/conhecimentos/css.png" alt="">
    </div>

    <div class="skill-div" data-skill="JavaScript">
      <img class="skill" src="../assets/conhecimentos/javascript.png" alt="">
    </div>

    <div class="skill-div" data-skill="TypeScript">
      <img class="skill" src="../assets/conhecimentos/typescript.png" alt="">
    </div>

    <div class="skill-div" data-skill="Java">
      <img class="skill" src="../assets/conhecimentos/java.png" alt="">
    </div>

    <div class="skill-div" data-skill="PHP">
      <img class="skill" src="../assets/conhecimentos/php.png" alt="">
    </div>

    <div class="skill-div" data-skill="Laravel">
      <img class="skill" src="../assets/conhecimentos/laravel.png" alt="">
    </div>

    <div class="skill-div" data-skill="MySQL">
      <img class="skill" src="../assets/conhecimentos/mysql.png" alt="">
    </div>

    <div class="skill-div" data-skill="VueJS">
      <img class="skill" src="../assets/conhecimentos/vuejs.png" alt="">
    </div>

    <div class="skill-div" data-skill="Vuetify">
      <img class="skill" src="../assets/conhecimentos/vuetify.png" alt="">
    </div>


  </div>
</div>

<div class="projects-div" id="projects">
  <h1 class="projects-title ma-15">Projects</h1>

  <div class="projetos-subdiv">
    <v-row>

      <v-col lg="4" sm="12" md="6">
        <div class="proj-div">
          <h3>Sicredi Front Copy</h3>
          <p>Front-end that mimics the "Become a Member" screen from Sicredi's website, built with VueJs and Vuetify.</p>
          <div class="text-center pa-4">
            <div class="text-center pa-4">
              <v-btn class="btn-style" @click="openDialog(3)">
                See more
              </v-btn>

              <v-dialog v-model="dialog[3]" width="auto">
                <v-card class="modal-project pa-6" max-width="800">
                  <v-btn
                    class="btn-close-modal ms-auto"
                    text="x"
                    @click="closeDialog(3)"
                  ></v-btn>
                  <v-card-title class="modal-title ma-3">Sicredi Front Copy</v-card-title>

                  <div class="spinner"></div>
                  <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/NVWHSnOj88Y?si=xiBinubfCQoTM6Pk?autoplay=1&muted=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                  </iframe>

                  <v-btn href="https://sicredi-front-vue-gustavo-cortezia-86b69n3ht.vercel.app" class="btn-project-modal mt-6 mb-3">Open Project</v-btn>
                </v-card>
              </v-dialog>
            </div>
          </div>
        </div>
      </v-col>

      <v-col lg="4" sm="12" md="6">
        <div class="proj-div">
          <h3>Crud Growdev Mentors</h3>
          <p>Crud to manage Growdev mentors, built with VueJs (front) and Laravel (back), and Vuetify for styling. It includes a complete CRUD with authentication, search bar, sorting, etc.</p>
          <div class="text-center pa-4">
            <v-btn class="btn-style" @click="openDialog(1)">
              See more
            </v-btn>

            <v-dialog v-model="dialog[1]" width="auto">
              <v-card class="modal-project pa-6" max-width="800">
                <v-btn
                  class="btn-close-modal ms-auto"
                  text="x"
                  @click="closeDialog(1)"
                ></v-btn>
                <v-card-title class="modal-title ma-3">Crud Growdev Mentors</v-card-title>

                <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/wtPWQOnMpFs?si=XRULaFYPPSEN8SrF?autoplay=1&muted=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn href="https://crud-mentores-gustavo-cortezia.vercel.app/" class="btn-project-modal mt-6 mb-3">Open Project</v-btn>
              </v-card>
            </v-dialog>
          </div>
        </div>
      </v-col>

      <v-col lg="4" sm="12" md="6">
        <div class="proj-div">
          <h3>Rick and Morty API</h3>
          <p>Listing and searching of characters from the Rick and Morty series using an API with HTML, CSS, Bootstrap, and JavaScript.</p>
          <div class="text-center pa-4">
            <v-btn class="btn-style" @click="openDialog(2)">
              See more
            </v-btn>

            <v-dialog v-model="dialog[2]" width="auto">
              <v-card class="modal-project pa-6" max-width="800">
                <v-btn
                  class="btn-close-modal ms-auto"
                  text="x"
                  @click="closeDialog(2)"
                ></v-btn>
                <v-card-title class="modal-title ma-3">Rick and Morty API</v-card-title>

                <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/crINiYif34Y?si=8cWUQIUC3qEKKlVm?autoplay=1&muted=1" title="YouTube video player" frameborder="0" allow="accelerometer autoplay clipboard-write encrypted-media gyroscope picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn href="https://rick-and-morty-three-livid.vercel.app/" class="btn-project-modal mt-6 mb-3">Open Project</v-btn>
              </v-card>
            </v-dialog>
          </div>
        </div>
      </v-col>

      <v-col lg="6" sm="12" md="6">
        <div class="proj-div">
          <h3>GrowTwitter</h3>
          <p>Application with VueJs and Laravel that mimics the social network "Twitter", with posts, likes, a tweets listing page, profile page, login with authentication, and much more. A group activity using git functionalities.</p>
          <div class="text-center pa-4">
            <v-btn class="btn-style" @click="openDialog(0)">
              See more
            </v-btn>

            <v-dialog v-model="dialog[0]" width="auto">
              <v-card class="modal-project pa-6" max-width="800">
                <v-btn
                  class="btn-close-modal ms-auto"
                  text="x"
                  @click="closeDialog(0)"
                ></v-btn>
                <v-card-title class="modal-title ma-3">GrowTwitter</v-card-title>

                <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/vbUeR-bH-iU?si=A4Y2KM1t6JbnzpjM?autoplay=1&muted=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn href="https://growtwitter-iota.vercel.app/login" class="btn-project-modal mt-6 mb-3">Open Project</v-btn>
              </v-card>
            </v-dialog>
          </div>
        </div>
      </v-col>

      <v-col lg="6" sm="12" md="12">
        <div class="proj-div">
          <h3>Find my Pet</h3>
          <p>Application that allows users to register lost animals with the goal of finding a home for them. Built with Laravel, HTML, CSS, and JavaScript.</p>
          <div class="text-center pa-4">
            <v-btn class="btn-style" @click="openDialog(4)">
              See more
            </v-btn>

            <v-dialog v-model="dialog[4]" width="auto">
              <v-card class="modal-project pa-6" max-width="800">
                <v-btn
                  class="btn-close-modal ms-auto"
                  text="x"
                  @click="closeDialog(4)"
                ></v-btn>
                <v-card-title class="modal-title ma-3">Find my Pet</v-card-title>

                <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/T_VZP8ZmwW8?si=vnxJPfU9JW6pUeq4?autoplay=1&muted=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn class="btn-project-modal mt-6 mb-3" disabled>In development</v-btn>
              </v-card>
            </v-dialog>
          </div>
        </div>
      </v-col>
    </v-row>
  </div>
</div>

<div class="soft-skills-div" id="soft-skills">
  <h1 class="soft-skill-title">Soft Skills</h1>

  <div class="soft-skills-subdiv">
    <div class="soft-skill">
      <h3 class="soft-title">Teamwork</h3>
      <p class="soft-text">I adapt very well to different team dynamics, often taking the role of leader. I like to ensure that all members are aligned and committed to the goals, creating a collaborative and productive environment.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Empathy</h3>
      <p class="soft-text">Understanding people's feelings is essential in leadership. I always try to put myself in other people's shoes to make the best decisions for the group, ensuring everyone feels heard and valued.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Creativity</h3>
      <p class="soft-text">When faced with challenges, I often come up with creative solutions to resolve problems in innovative ways, contributing fresh ideas and perspectives to the team.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Problem-solving</h3>
      <p class="soft-text">One of my strongest points is solving problems efficiently. I like to analyze situations and explore all possible solutions to find the best approach, always aiming for effective results.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Emotional Intelligence</h3>
      <p class="soft-text">In high-pressure situations, I manage to maintain calm and help guide the team through challenges with a focus on emotional balance, ensuring we don't lose sight of our goals.</p>
    </div>

    <div class="soft-skill">
  <h3 class="soft-title">Social Skills</h3>
  <p class="soft-text">My social skills are a key factor for success in teamwork. I enjoy building good relationships with group members, which facilitates communication and collaboration, resulting in a more positive and efficient work environment.</p>
</div>

<div class="soft-skill">
  <h3 class="soft-title">Advanced English</h3>
  <p class="soft-text">My advanced English proficiency allows me to work in international teams and participate in complex discussions, translating ideas and instructions with clarity and precision. It also enhances my leadership opportunities in global projects.</p>
</div>

<div class="soft-skill">
  <h3 class="soft-title">Determination and Commitment</h3>
  <p class="soft-text">My determination drives me to always seek the best results for the team. As a leader, I am committed to ensuring that everyone stays focused and motivated to achieve the set goals, guiding the group toward the successful completion of tasks.</p>
</div>

</div>
</div>

<div class="contacts-div" id="contacts">
  <h1 class="contact-title">Contact</h1>

  <div class="contacts-subdiv">

    <div class="contact">
      <a href="mailto:gus.cortezia@gmail.com" target="_blank">
        <img class="contact-img" src="../assets/conhecimentos/email-img.png" alt="">
      </a>
      <h3 class="mt-4">Email</h3>
      <p>gus.cortezia@gmail.com</p>
    </div>

    <div class="contact">
      <a href="https://www.linkedin.com/in/gustavocortezia/" target="_blank">
        <img class="contact-img" src="../assets/conhecimentos/linkedin-img.png" alt="">
      </a>
      <h3 class="mt-4">LinkedIn</h3>
      <p>Gustavo Cortezia</p>
    </div>

    <div class="contact">
      <a href="https://api.whatsapp.com/send?phone=5551992329545" target="_blank">
        <img class="contact-img" src="../assets/conhecimentos/whatsapp-img.png" alt="">
      </a>
      <h3 class="mt-4">WhatsApp</h3>
      <p>+55 51 99232-9545</p>
    </div>

    <div class="contact">
      <a href="https://github.com/GustavoCortezia" target="_blank">
        <img class="contact-img" src="../assets/conhecimentos/github-img.png" alt="">
      </a>
      <h3 class="mt-4">GitHub</h3>
      <p>GustavoCortezia</p>
    </div>

  </div>
</div>

<footer>

</footer>






</v-app>
</template>

<style>

  .nav-title{
    font-weight: bold !important;
    font-size: 1.6rem !important;
    margin-left: 50px !important;
  }

  .gustavo-nome {
    font-size: 5rem;
  }

  .home-bg {
    width: 100%;
    height: 800px;
    display: flex;
    align-items: center;
    justify-content: space-around;

  }

  .minha-foto {
    border: 5px solid rgb(17, 100, 209);
    position: relative;
    transition: transform 0.4s, box-shadow 0.8s !important;
  }

  .minha-foto:hover {
    box-shadow: 0px 0px 66px -10px  rgb(17, 100, 209);
    transform: scale(0.95);
  }

  .home-text {
    color: rgb(17, 100, 209);
    font-size: 1.6rem;
  }

  .home-text-div {
    width: 100%;
    text-align: center;
    justify-content: center;
    flex-direction: column;
    align-items: center !important;
  }

  .col {
    display: flex;
    align-items: center
  }

  .img-div {
    width: 100%;
    display: flex;
    justify-content: center;
  }

  .about-card {
    border-radius: 1rem !important;
    width: 70%;
    height: 97%;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px;
  }

  .about-card-text {
    font-size: 1.5rem;
    text-align: justify;
  }

  .about-div {
    display: flex;
    justify-content: center;

  }

  .about-card-title {
    font-size: 2rem;
    color: rgb(17, 100, 209);
    font-weight: 1000;
    margin-bottom: 1rem;
  }

  .educacao {
    width: 100%;
    height: 900px;
    background-color: rgb(31, 31, 31);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }

  .education-title {
    color: rgb(17, 100, 209);
    font-size: 3rem;
    letter-spacing: 2px;
  }

  .educ-card-title{
    font-size: 1.8rem !important;
    margin-top: -8px;
  }

  .col-educ{
    display: flex !important;
    justify-content: center !important;
    align-items: center !important;

  }

  .grow-div{
    height: 500px;
  }

  .unisinos-card {
    background-color: rgb(23, 23, 23) !important;
    border-left: 5px solid rgb(31, 31, 31) !important ;
    transition: border 0.5s !important;
    margin-inline: 40px !important;
  }

  .unisinos-card:hover{
    border-left: 5px solid rgb(17, 100, 209) !important;
  }

  @media (max-width: 960px) {
      .educacao{
        height: 1500px;
      }

      .div-container{
        display: flex !important;
        align-items: center !important;
      }
  }


  .grow-card{
    margin-top: 100px;
    display: flex !important;
    border-top: 5px solid rgb(17, 100, 209) !important;
    border-radius: 20px !important;
    position: relative;
    transition: transform 0.4s !important;
    width: 90% !important;
    height: 91% !important;
  }

  @media (max-width: 1645px) {
    .grow-card{
      height: 100% !important;
    }
    .grow-img{
      width: 40% !important;
      height: 100% !important;
    }
  }



  @media (max-width: 1440px) {
    .grow-card {
      flex-direction: column !important;
      width: 45% !important;
      height: auto !important;
    }
    .grow-img {
      width: 100% !important;
      height: auto !important; /* Ajusta a imagem para se redimensionar automaticamente */
    }
    .grow-content {
      display: flex;
      justify-content: center;
      flex-direction: column;
      align-items: center;
      width: 90% !important;
      height: auto !important;
      padding: 20px !important;
    }

    .title-grow-card{
      text-align: center;
    }

    .conhecimentos-div{
      margin-top: 800px !important;
    }


    .soft-skills-div{
      margin-top: 500px;
    }

    .contacts-div{
      margin-top: 500px !important;
    }
  }

  .grow-card:hover {
    transform: scale(1.03);
  }

  .grow-content{
    padding: 30px;
    text-align: justify;
    margin-inline: 25px;

  }

  .despertar-dev{
    color: rgb(17, 100, 209);
  }

  .conhecimentos-div {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 800px;
  margin-top: 100px;
}

.conhecimentos {
  height: 400px;
  width: 1050px;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-template-rows: repeat(2, 1fr);
  justify-items: center;
  align-items: center;
}

@media (max-width: 1140px ) {
  .conhecimentos{
    grid-template-columns: repeat(4, 1fr);
  }
}

.skill {
  width: 100px;
}

.skill-div {
  border: 3px solid rgb(31, 31, 31);
  border-radius: 10%;
  width: 150px;
  height: 150px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin: 15px;
  background-color: rgb(31, 31, 31);
  position: relative;
  transition: transform 0.4s, border 0.4s;
}

.skill-div:hover {
  border: 3px solid rgb(17, 100, 209);
  transform: scale(1.1);
}

.skill-div:after {
  content: attr(data-skill);
  position: absolute;
  bottom: -33px;
  font-size: 1.2rem;
  color: rgb(17, 100, 209);
  opacity: 0;
  transition: opacity 0.3s;
}


.skill-div:hover:after {
  opacity: 1;
}

.conhecimentos-title {
  font-size: 2.7rem;
  color: rgb(17, 100, 209);
}

.nav {
  border-bottom: 2px solid rgb(17, 100, 209) !important;
  background-color: rgb(18, 18, 18) !important;
}

.projects-div{
  border-top: rgb(17, 100, 209) 2px solid;
  border-bottom: solid rgb(17, 100, 209) 2px;
  background-color: rgb(25, 25, 25);
  height: 1000px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}


.projects-title {
  color: rgb(17, 100, 209);
  margin-top: 70px !important;
  font-size: 2.6rem;
  text-align: center;
}

.projetos-subdiv {
  width: 75%;
  padding: 20px;
}

.proj-div {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 250px;
  border: 3px solid rgb(17, 100, 209);
  border-radius: 10px;
  padding: 20px !important;
  margin-top: 10px !important;
  transition: transform 0.3s;
}

.proj-div:hover {
  transform: scale(1.03); /* Efeito ao passar o mouse */
}

/* Responsividade */
@media (max-width: 768px) {
  .proj-div {
    width: 100%; /* Ocupa toda a largura disponível em telas pequenas */
    height: auto;
    padding: 15px;
  }

  .projects-title {
    font-size: 2rem;
  }

  .projetos-subdiv {
    flex-direction: column;
    align-items: center;
  }
}

@media (max-width: 480px) {
  .projects-title {
    font-size: 1.8rem;
  }
}


.modal-project{
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 20px !important;
}

.video-player-tag{
  border-radius: 10px;
}

.modal-title {
  color: rgb(17, 100, 209);
  font-size: 1.6rem !important;
}

.btn-close-modal{
  margin-bottom: -40px;
  margin-top: -5px;
  margin-right: -15px;
  width: 10px !important;
  box-shadow: none !important;
  border-radius: 50px !important;
}

.btn-close-modal:hover{
  color: red;
}

.btn-project-modal{
  color: rgb(17, 100, 209) !important;
  border: 1px solid rgb(17, 100, 209) !important;
}

.btn-project-modal:hover{
  color: rgb(18, 18, 18) !important;
  border: 1px solid rgb(18, 18, 18) !important;
  background-color: rgb(17, 100, 209);
}

.soft-skills-div{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  height: 1000px;
}

.soft-skill {
  border: 1px solid white;
  border-radius: 5px;
  width: 300px;
  height: 350px;
  padding: 30px;
  transition: border 0.3s;
}

.soft-skill:hover {
  border: 1px solid rgb(17, 100, 209);
}

.soft-skills-subdiv{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  width: 80%;
  gap: 50px;
}

.soft-skill-title{
  margin: 100px !important;
  color: rgb(17, 100, 209);
}

.soft-title{
  color: rgb(17, 100, 209);
  font-size: 1.3rem;
  margin: 10px;
}

.contacts-div{
  display: flex;
  justify-content: center !important;
  align-items: center;
  width: 100%;
  height: 800px;
  flex-direction: column;
  margin-top: 150px;
}

.contacts-subdiv{
  display: flex;
  justify-content: center !important;
  align-items: center;
  gap: 100px;
  width: 100%;
  height: 350px;
}

.contact-img{
  width: 100px;
}

.contact{
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  padding: 30px;
  border-radius: 100% ;
  transition: transform 0.3s;
}

.contact:hover{
  transform: scale(1.10);
}

.contact-tilte {
  color: rgb(17, 100, 209);
  font-size: 2.5rem;
  margin-bottom: 50px;
  margin-top: 80px;
}

.spinner {
      border: 8px solid #f3f3f3;
      border-top: 8px solid rgb(17, 100, 209);
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: spin 1s linear infinite;
      position: fixed;
      z-index: -1;
      /* margin: 100px auto; */
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    .btn-lingua{
      width: 30px !important;
      height: 55px !important;
    }

    .btn-lingua:hover{
      border-radius: 100% !important;
    }




@media (max-width: 1280px) {
  .conhecimentos{
    width: 90%;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, 1fr);
  }

  .conhecimentos-div{
    height: 1000px;
  }

  .contacts-subdiv{
    flex-wrap: wrap;
    gap: 90px;
  }

  .home-text-div{
    width: 90%;
  }

  .projects-div{
    height: 1500px;
  }

  .proj-div{
    width: 100%;
    height: 100%;
  }

  .minha-foto{
    width: 300px ;
    height: 300px;
  }

  .gustavo-nome{
    font-size: 3rem;
  }

  .col{
    display: flex;
    justify-content: center;
  }

  .grow-card{
    width: 70% !important;
  }
}

@media (max-width: 900px) {
  .projects-div{
    height: 1650px;
  }
}

@media (max-width: 817px) {
  .conhecimentos{
    width: 90%;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
  }

  .grow-div{
    height: 1400px !important;
  }

  .v-card {
    max-width: 100% !important;
    max-height: 100% !important;
  }

  .modal-project {
  width: 100% !important;
  height: 100% !important;
}

.v-overlay__content {
  justify-content: center;
  align-items: center;
  width: 100vw !important;
  max-width: 97vw !important;
  height: 97vh !important;
  max-height: 100vh !important;
}

.btn-close-modal{
  margin-bottom: 10px;
}

.video-player-tag{
  width: 100% !important;
}

  .education-title{
    font-size: 2rem;
  }

  .title-grow-card{
    font-size: 1.6rem;
    text-align: center;
  }

  .minha-foto{
    margin-top: 50px;
  }

  .home-bg{
    height: 1000px;
  }

  .conhecimentos-div{
    height: 1400px;
    margin-top: 0 !important;
  }

  .grow-card{
    width: 90% !important;
  }

  .about-div{
    width: 100% !important;
    margin: 0 !important;
  }

  .about-card{
    margin: 0 !important;
    width: 100% !important;
    padding: 20px !important;
  }

  .about-card-text{
    text-align: center;
  }

  .projects-div{
    height: 1650px;
  }

  .soft-skills-div{
    height: 2400px;
  }

}

@media (max-width: 575px) {
  .conhecimentos{
    width: 80%;
    height: 700px !important;
    grid-template-columns: repeat(2, 1fr);
  }

  .skill-div{
    margin-bottom: 25px;
  }

  .conhecimentos-div{
    height: 1400px !important;
    margin-top: 0 !important;
  }

  .projects-div{
    height: 2300px !important;
  }

  .unisinos-card{
    width: 400px !important;
    margin: 0 !important;
  }

  .btn-style{
    font-size: 0.6rem;
  }


.col-educ{
    width: 200px !important;
    padding: 00px !important;
  }

  .projects-div{
    height: 1900px;
  }

  /* .grow-div{
    height: 300px;
  } */

  .contacts-div{
    height: 2200px;
    margin-top: 100px !important;
  }

  .minha-foto{
    height: 200px;
    width: 200px;
  }

}

@media (max-width: 480px) {
  .conhecimentos{
    grid-template-columns: repeat(2, 1fr);
  }

  .skill-div{
    width: 120px;
    height: 120px;
  }

  .conhecimentos-div{
    height: 2000px !important;
    margin-top: 0 !important;
  }

  .about-card {
    border-radius: 1rem !important;
    width: 70%;
    height: 99%;
  }
  .about-div{
    margin: 0 !important;
  }

  .col-educ{
    width: 200px !important;
    padding: 00px !important;
  }

  .projects-div{
    height: 2000px;
  }

    .grow-div{
    height: 250px;
  }
}

h3{
  margin: 10px;
}

.unisinos_vista_img{
  width: 250px;
  height: 250px;
  border-radius: 50%;
  border: 2px solid white;
}

.modal-education{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 400px;
  height: 600px;
  border-radius: 5% !important;
}

.habilidades-desenvolvidas{
  text-align: center;
}

@media (max-width: 445px) {
  .modal-education{
    width: 100% !important;
    margin: 0 !important;
  }
  .unisinos_vista_img{
  width: 200px;
  height: 200px;
}

.unisinos-card{
    width: 200px !important;
  }

  .col-educ {
  /* Remova o width e padding forçado */
  width: 100% !important;
  padding: 0 !important;
}
}

@media (max-width: 1150px) {
  .nav-btns{
    display: none !important;
  }
  .nav-title{
    margin-left: 15px !important;
  }

}

.btn-style{
  color: rgb(17, 100, 209);
}

.btn-style:hover{
  background-color: rgb(17, 100, 209);
  color: white;
}

@media (max-width: 578px) {
  .col-educ{
    width: 100% !important;
  }

  .uni-img{
    width: 100% !important;
  }

  .unisinos-card{
    width: 80% !important;
  }
}

.education-title{
  text-align: center;
}

@media (min-width: 1440px) and (max-width: 1690px) {
  .soft-skills-div{
    height: 1400px;
  }
}
</style>



