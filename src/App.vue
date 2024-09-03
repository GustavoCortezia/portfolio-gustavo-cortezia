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
  <h1 class="education-title ma-15">Education</h1>

  <v-row>
    <v-col></v-col>
    <v-col></v-col>
  </v-row>

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
    height: 500px;
    background-color: rgb(31, 31, 31);
    display: flex;
    justify-content: center;
  }

  .education-title {
    color: rgb(17, 100, 209);
    font-size: 2.8rem;
  }
</style>
