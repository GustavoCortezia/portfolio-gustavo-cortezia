  <script lang="ts" setup>
    //
  </script>


<template>
  <v-app>
    <v-app-bar :elevation="3">
  <template v-slot:prepend>
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
  </template>

  <v-app-bar-title>Gustavo Cortezia</v-app-bar-title>

  <template v-slot:append>
    <v-btn icon="mdi-heart"></v-btn>

    <v-btn icon="mdi-magnify"></v-btn>

    <v-btn icon="mdi-dots-vertical"></v-btn>
  </template>
</v-app-bar>

<div class="home-bg">
  <v-row class="mx-15">
    <v-col md="6" sm="12" class="col">
      <div class="img-div">
        <img class="minha-foto rounded-circle" width="400px" height="400px" src="./assets/Captura de tela 2024-07-15 144029.png" alt="">
      </div>
    </v-col>

    <v-col md="6" sm="12" class="col">
      <div class="home-text-div d-flex">

        <h1 class="gustavo-nome mb-6">Gustavo Cortezia</h1>

        <p class="home-text"> Web Full Stack Developer | Computer Science | VueJS | Laravel | MySQL | PHP | JavaScript | TypeScript | Java | HTML | CSS</p>
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
    I have knowledge in HTML, CSS, JavaScript, Java, PHP, Laravel, Bootstrap, TypeScript, VueJS, Vuetify and MySQL. Besides, some of my strengths are social skills, creativity, emocional intelligence and problem solving. I am a very determined and committed person and I’m always looking forward to a better future.
  </p>
</v-card-text>

</v-card>
</div>

<div class="educacao">
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
    </div>


  </v-card>

</div>


  <div class="conhecimentos-div">
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





  </v-app>

</template>

<style>

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
  }

  .minha-foto:hover {
    border: 5px solid white;
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
    height: 450px;
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
    border-left: 10px solid rgb(17, 100, 209) !important;
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

</style>
