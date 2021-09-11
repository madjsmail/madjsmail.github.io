<template>
  <div class="Portfolio">

    <div class="container container-Portfolio">
      <h1 class="upercase">
        my work
      </h1>

      <div class="card" v-for="(work, index) in works" v-bind:key="index">
        <div class="card-content">
          <h3 class="upercase">{{ work.title }}</h3>
          <p v-html="work.body"></p>
        </div>
        <div class="card-img">
          <img :src="work.photo" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      active: false,
      works: [
        {
          title: "moadaly",
          body: `is a web application that allow you to calculate your pass mark. The app is for first and second year computer science student " LMD "
تطبيق ويب لحساب المعدل الفصلي و السنوي للسنة الاولى و الثانية اعلام الى نطام
     <br/>
            <a href="https://abdelmadjidsmail.github.io/moadaly/ " target="_" class="links about-link "> demo  </a>
            <a href="https://github.com/Abdelmadjidsmail/moadaly" target="_"  class="links about-link"> code source </a>
            <br/>
            <b>Languages :</b> <span class="upercase" > HTML</span> 
             <span class="upercase" > css</span> 
             <span class="upercase" > javascript </span> 
             <span class="upercase" > scss</span> 
            `,
          photo: require("../assets/moadly.jpg")
        },
        {
          title: "tasnif",
          body: `An app that allows the user to search for scientific journals with their classifications.
     <br/>
            <a href="http://tahadz.com/tasnif/" target="_" class="links about-link "> demo  </a>
            <a href="https://github.com/40uf411/Tasnif" target="_"  class="links about-link"> code source </a>
            <br/>
            <b>Languages :</b> <span class="upercase" > HTML</span> 
             <span class="upercase" > css</span> 
             <span class="upercase" > javascript </span> 
            `,
          photo: require("../assets/tasnif.jpg")
        },
        {
          title: "GED SETRAM",
          body: `Document Management System for the company setram. <br/>
            <b>Languages :</b> <span class="upercase" > HTML</span> 
             <span class="upercase" > css</span> 
             <span class="upercase" > javascript </span> 
             <span class="upercase" > php /laravel </span> 
          `,
          photo: require("../assets/setram.png")
        },
        {
          title: "Awalna",
          body: `dictionary for the Algerian dialect built with vuejs and firebase. <br/>
            <a href="https://awalna-76bf8.firebaseapp.com/" target="_" class="links about-link "> demo  </a>
            <a href="https://github.com/Abdelmadjidsmail/darja" target="_"  class="links about-link"> code source </a><br/>
            <b>Languages :</b> <span class="upercase" > HTML</span> 
             <span class="upercase" > css</span> 
             <span class="upercase" > javascript /vuejs </span> 
             <span class="upercase" > firebase </span> 

          `,
          photo: require("../assets/awalna.jpg")
        }
      ]
    };
  },
  created() {
    this.active = true;
  }
};
</script>

<style></style>
