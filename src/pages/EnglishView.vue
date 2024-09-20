<script lang="ts" setup>
import { ref } from 'vue';
import { useRouter } from 'vue-router';


  const dialog = ref<boolean>(false);
    const router = useRouter();

function portugues(){
  router.push('/');
}
  </script>


<template>
  <v-app>
    <v-app-bar :elevation="3" class="nav">

  <v-app-bar-title class="nav-title">Gustavo Cortezia
     <v-btn @click="portugues" class="ml-4 btn-lingua"><img src="./assets/brasil_circulo.png" alt="" width="51px"></v-btn>
     <v-btn class="btn-lingua"><img src="./assets/USAworld_flags_6_-512.webp" alt="" width="33px"></v-btn>
    </v-app-bar-title>



  <v-btn href="#about-me">About Me</v-btn>

<v-btn href="#education">Education</v-btn>

<v-btn href="#hard-skills">Hard Skills</v-btn>

<v-btn href="#soft-skills">Soft Skills</v-btn>

<v-btn href="#projects">Projects</v-btn>

<v-btn href="#contacts">Contacts</v-btn>


</v-app-bar>

<div class="home-bg">
  <v-row class="mx-15">
    <v-col md="6" sm="12" class="col">
      <div class="img-div">
        <a href="https://www.linkedin.com/in/gustavocortezia/" target="_blank">
    <img class="minha-foto rounded-circle" width="400px" height="400px" src="./assets/Captura de tela 2024-07-15 144029.png" alt="Minha Foto">
  </a>
      </div>
    </v-col>

    <v-col md="6" sm="12" class="col">
      <div class="home-text-div d-flex">

        <h1 class="gustavo-nome mb-6">Gustavo Cortezia Ingles</h1>

        <p class="home-text" id="about-me"> Web Full Stack Developer | Computer Science | VueJS | Laravel | MySQL | PHP | JavaScript | TypeScript | Java | HTML | CSS</p>
        </div>
    </v-col>
  </v-row>


</div>

<div class="about-div ma-10">
  <v-card class="about-card pa-10" min-width="700px">

<v-card-title >
  <p class="about-card-title">
    About Me
  </p>
</v-card-title>

<v-card-text>
  <p class="about-card-text">
    I’ve been studying Computer Science at Unisinos University. I was also selected by Sicredi Pioneira, one of the largest financial institutions in Latin America to study Web Full Stack Development at Growdev, a tecnology school that trains professionals for the digital product market. I studied all my elementary and high school at Colégio Sinodal, one of the best schools in Rio Grande do Sul.
  </p>
</v-card-text>

<v-card-text>
  <p class="about-card-text">
    Tenho conhecimento em HTML, CSS, JavaScript, Java, PHP, Laravel, Bootstrap, TypeScript, VueJS, Vuetify e MySQL. Além disso, alguns dos meus pontos fortes são habilidades sociais, criatividade, inteligência emocional, resolução de problemas e inglês avançado. Sou uma pessoa muito determinada e comprometida e estou sempre em busca de um futuro melhor.
  </p>
</v-card-text>

</v-card>
</div>

<div class="educacao" id="education">
  <h1 class="education-title mb-15 mt-n10" >My Education</h1>

<v-container>

  <v-row class="div-container">
    <v-col md="6" sm="12" class="col-educ">
      <v-card
      class="unisinos-card mx-auto mr-15"
      width="400"
      height="550"
    >
      <v-img
        class="align-end text-white"
        height="300"
        width="400"
        src="./assets/image.png"
        cover
      >
    </v-img>
    <div class="pa-5">
      <v-card-title class="educ-card-title">Unisinos University</v-card-title>

        <v-card-text>
          <h2>Computer Science</h2>
          <h3 class="mb-5"> (03/2023 - now)</h3>


          <h4>Main Skills: Emocional intelligence, Algorithms, Innovation, Agile Enviroment, Databases, Software Engineering, Java  </h4>
        </v-card-text>
    </div>

    </v-card>
  </v-col>



    <v-col md="6" sm="12" class="col-educ">
      <v-card
      class="unisinos-card mx-auto ml-15"
      width="400"
      height="550"
    >
      <v-img
        class="align-end text-white"
        height="300"
        width="400"
        src="./assets/logosinodalquadrado.webp"
        cover
      >
    </v-img>
    <div class="pa-5">
    <v-card-title class="educ-card-title">Colégio Sinodal</v-card-title>

    <v-card-text>
      <h2>Educação Básica</h2>
        <h3 class="mb-5">(2006 - 2022)</h3>

        <h4>Main Skills: Problem Solving, Creativity, Leadership, Creative Writing, Teamwork  </h4>
      </v-card-text>
    </div>
    </v-card>
  </v-col>
  </v-row>
</v-container>

</div>


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
      src="./assets/growdev-logo-branco.png"
      cover
    ></v-img>
    <div class="grow-content">
      <h1 class="ma-5 mb-10">Starter Growdev Program - <span class="despertar-dev">Despertar.dev</span></h1>

    <h3>O Programa Starter Full Stack Developer é uma formação completa que vai dos fundamentos da programação e tecnologia até o desenvolvimento de um software completo com front-end, back-end, banco de dados, cache, com qualidade garantida com testes automatizados e a disponibilização (deploy) do sistema em produção. Além disso, os alunos têm a oportunidade de aplicar os seus conhecimentos em projetos contratados por empresas, desenvolvidos na fábrica de software da Growdev.</h3>
<br>
    <h3>Fui selecionado pela<span class="despertar-dev"> Sicredi Pioneira</span>, por meio de um processo seletivo, para ganhar uma bolsa de estudos (100%) para o Starter Growdev Program, do qual me garantiu muito aprendizado e experiência </h3>
    <h3>Carga Horária: 1000 horas</h3>
    </div>


  </v-card>

</div>


  <div class="conhecimentos-div" id="hard-skills">
  <h1 class="conhecimentos-title mb-15">Conhecimentos</h1>


  <div class="conhecimentos">

    <div class="skill-div" data-skill="HTML">
      <img class="skill" src="./assets/conhecimentos/html.png" alt="">
    </div>

    <div class="skill-div"  data-skill="CSS">
      <img class="skill" src="./assets/conhecimentos/css.png" alt="">
    </div>

    <div class="skill-div" data-skill="JavaScript">
      <img class="skill" src="./assets/conhecimentos/javascript.png" alt="">
    </div>

    <div class="skill-div" data-skill="TypeScript">
      <img class="skill" src="./assets/conhecimentos/typescript.png" alt="">
    </div>

    <div class="skill-div" data-skill="Java">
      <img class="skill" src="./assets/conhecimentos/java.png" alt="">
    </div>

    <div class="skill-div" data-skill="PHP">
      <img class="skill" src="./assets/conhecimentos/php.png" alt="">
    </div>

    <div class="skill-div" data-skill="MySQL">
      <img class="skill" src="./assets/conhecimentos/mysql.png" alt="">
    </div>

    <div class="skill-div" data-skill="Laravel">
      <img class="skill" src="./assets/conhecimentos/laravel.png" alt="">
    </div>

    <div class="skill-div" data-skill="VueJS">
      <img class="skill" src="./assets/conhecimentos/vuejs.png" alt="">
    </div>

    <div class="skill-div" data-skill="Vuetify">
      <img class="skill" src="./assets/conhecimentos/vuetify.png" alt="">
    </div>
  </div>
  </div>

    <div class="projects-div" id="projects">
      <h1 class="projects-title ma-15">Projects</h1>

      <div class="projetos-subdiv">

      <v-row>


        <v-col lg="4">
          <div class="proj-div">
            <h3>Cópia Sicredi Front</h3>
            <p>Front-end que imita a tela "Seja Associado" do site do Sicredi, com VueJs e Vuetify </p>
            <div class="text-center pa-4">
              <v-btn @click="dialog = true">
                Ver mais
              </v-btn>

              <v-dialog
                v-model="dialog"
                width="auto"
              >
              <v-card class="modal-project pa-6" max-width="800">
                  <v-btn
                      class="btn-close-modal ms-auto"
                      text="x"
                      @click="dialog = false"
                    ></v-btn>
                  <v-card-title class="modal-title ma-3">Cópia Sicredi Front</v-card-title>

                  <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/W8Y-pKCKZNU"
                title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn class="btn-project-modal mt-6 mb-3">Abrir Projeto</v-btn>

                </v-card>
              </v-dialog>
            </div>
          </div>
        </v-col>


        <v-col lg="4">
          <div class="proj-div">
            <h3>Crud Mentores Growdev</h3>
            <p>Crud que gerencia mentores da Growdev, feita com VueJs (front) e Laravel (back), além do Vuetify para os estilos. Contém um crud completo com autenticação, barra de pesquisa, ordenação, etc.</p>
            <div class="text-center pa-4">
              <v-btn @click="dialog = true">
                Ver mais
              </v-btn>

              <v-dialog
                v-model="dialog"
                width="auto"
              >
              <v-card class="modal-project pa-6" max-width="800">
                  <v-btn
                      class="btn-close-modal ms-auto"
                      text="x"
                      @click="dialog = false"
                    ></v-btn>
                  <v-card-title class="modal-title ma-3">Crud Mentores Growdev</v-card-title>

                  <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/W8Y-pKCKZNU"
                title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn class="btn-project-modal mt-6 mb-3">Abrir Projeto</v-btn>

                </v-card>
              </v-dialog>
            </div>
          </div>
        </v-col>

        <v-col lg="4">
          <div class="proj-div">
            <h3>API Rick and Morty</h3>
            <p>Listagem e pesquisa dos personagens da serie Rick and Morty de uma API utilizando HTMl, CSS, Bootsrap e Javascript.</p>
            <div class="text-center pa-4">
              <v-btn @click="dialog = true">
                Ver mais
              </v-btn>

              <v-dialog
                v-model="dialog"
                width="auto"
              >
              <v-card class="modal-project pa-6" max-width="800">
                  <v-btn
                      class="btn-close-modal ms-auto"
                      text="x"
                      @click="dialog = false"
                    ></v-btn>
                  <v-card-title class="modal-title ma-3">API Rick and Morty</v-card-title>

                  <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/W8Y-pKCKZNU"
                title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn class="btn-project-modal mt-6 mb-3">Abrir Projeto</v-btn>

                </v-card>
              </v-dialog>
            </div>
          </div>
        </v-col>

        <v-col lg="6">
          <div class="proj-div">
            <h3>GrowTwitter</h3>
            <p>Aplicação com VueJs e Laravel que imita a rede social "Twitter", com postagens, curtidas, listagem de tweets, página de perfil, login com autenticação e muito mais. Atividade feita em conjunto utilizando as funcionalidades git</p>
            <div class="text-center pa-4">
              <v-btn @click="dialog = true">
                Ver mais
              </v-btn>

              <v-dialog
                v-model="dialog"
                width="auto"
              >
              <v-card class="modal-project pa-6" max-width="800">
                  <v-btn
                      class="btn-close-modal ms-auto"
                      text="x"
                      @click="dialog = false"
                    ></v-btn>
                  <v-card-title class="modal-title ma-3">GrowTwitter</v-card-title>

                  <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/W8Y-pKCKZNU"
                title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn class="btn-project-modal mt-6 mb-3">Abrir Projeto</v-btn>

                </v-card>
              </v-dialog>
            </div>
          </div>
        </v-col>

        <v-col lg="6">
          <div class="proj-div">
            <h3>Find my Pet</h3>
            <p>Aplicação que permite o usuário cadastrar animais perdidos com o objetivo de encontrar um lar para eles. Feito com Laravel, HTML, CSS e Javascript</p>
            <div class="text-center pa-4">
              <v-btn @click="dialog = true">
                Ver mais
              </v-btn>

              <v-dialog
                v-model="dialog"
                width="auto"
              >
              <v-card class="modal-project pa-6" max-width="800">
                  <v-btn
                      class="btn-close-modal ms-auto"
                      text="x"
                      @click="dialog = false"
                    ></v-btn>
                  <v-card-title class="modal-title ma-3">Find my Pet</v-card-title>

                  <div class="spinner"></div>
                <iframe class="video-player-tag" width="560" height="315" src="https://www.youtube.com/embed/W8Y-pKCKZNU"
                title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
                </iframe>

                <v-btn class="btn-project-modal mt-6 mb-3">Abrir Projeto</v-btn>

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
      <h3 class="soft-title">Trabalho em grupo</h3>
      <p class="soft-text">Consigo me adaptar muito bem a diferentes dinâmicas de equipe, assumindo frequentemente o papel de líder. Gosto de garantir que todos os membros estejam alinhados e comprometidos com os objetivos, criando um ambiente colaborativo e produtivo.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Empatia</h3>
      <p class="soft-text">Minha habilidade de me colocar no lugar dos outros facilita a criação de um ambiente de confiança e respeito no grupo. Sempre busco compreender as perspectivas e sentimentos dos colegas, o que me ajuda a mediar conflitos e promover harmonia.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Criatividade</h3>
      <p class="soft-text">Quando lidero, busco inspirar o grupo a pensar "fora da caixa" e explorar soluções inovadoras. Minha abordagem criativa ajuda a identificar oportunidades que podem não ser evidentes à primeira vista, especialmente em situações complexas.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Resolução de problemas</h3>
      <p class="soft-text">Tenho uma abordagem proativa e analítica para resolver problemas. Como líder, incentivo a equipe a explorar diferentes caminhos e chegar a soluções eficazes, sempre mantendo o foco nos resultados.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Inteligência emocional</h3>
      <p class="soft-text">Com uma alta inteligência emocional, sei gerenciar bem as emoções tanto em mim quanto nos outros. Isso é crucial durante momentos de pressão no grupo, onde consigo manter a calma e motivar os colegas a seguir em frente.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Habilidades Sociais</h3>
      <p class="soft-text">Minhas habilidades sociais são uma peça-chave para o sucesso no trabalho em equipe. Gosto de construir boas relações com os membros do grupo, o que facilita a comunicação e a colaboração, resultando em um ambiente de trabalho mais positivo e eficiente.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Inglês Avançado</h3>
      <p class="soft-text">O domínio avançado do inglês me permite atuar em equipes internacionais e participar de discussões complexas, traduzindo ideias e orientações com clareza e precisão. Isso também amplia minhas oportunidades de liderança em projetos globais.</p>
    </div>

    <div class="soft-skill">
      <h3 class="soft-title">Determinação e Comprometimento</h3>
      <p class="soft-text">Minha determinação me impulsiona a buscar sempre os melhores resultados para a equipe. Como líder, me comprometo a garantir que todos estejam focados e motivados a alcançar os objetivos definidos, guiando o grupo até a conclusão bem-sucedida das tarefas.</p>
    </div>

  </div>
</div>





<div class="contacts-div" id="contacts">
  <h1 class="contact-tilte">Contato</h1>

  <div class="contacts-subdiv">

      <div class="contact">
        <a href="mailto:gus.cortezia@gmail.com" target="_blank">
          <img class="contact-img" src="./assets/conhecimentos/email-img.png" alt="">
        </a>
        <h3 class="mt-4">E-mail</h3>
        <p>gus.cortezia@gmail.com</p>
      </div>

      <div class="contact">
        <a href="https://www.linkedin.com/in/gustavocortezia/" target="_blank">
          <img class="contact-img" src="./assets/conhecimentos/linkedin-img.png" alt="">
        </a>
        <h3 class="mt-4">Linkedin</h3>
        <p>Gustavo Cortezia</p>
      </div>

      <div class="contact">
        <a href="https://api.whatsapp.com/send?phone=5551992329545" target="_blank">
          <img class="contact-img" src="./assets/conhecimentos/whatsapp-img.png" alt="">
        </a>
        <h3 class="mt-4">Whatsapp</h3>
        <p>+55 51 99232-9545</p>
      </div>

      <div class="contact">
        <a href="https://github.com/GustavoCortezia" target="_blank">
          <img class="contact-img" src="./assets/conhecimentos/github-img.png" alt="">
        </a>
        <h3 class="mt-4">Github</h3>
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
    width: 750px;
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
    height: 100%;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px;
  }

  .about-card-text {
    font-size: 1.5rem;
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
    margin-top: 90px;
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
</style>

