<template>
  <div class="container  ">
    <h1 class="upercase">
      my work
    </h1>
    <section class="card-list">
      <!-- <article class="card">
        <header class="card-header">
          <img src="../assets/moadly.jpg" alt="" />
        </header>
        <main class="card-content">
          <h2>
            title : balasas
          </h2>
          <p>
            description
          </p>
        </main>
        <div class="card-footer"></div>
      </article> -->
      <div class="card" v-for="(work, index) in works" v-bind:key="index">
        <div class="card-content">
          <h3 class="upercase">{{ work.title }}</h3>
          <p v-html="work.body"></p>
        </div>
        <div class="card-img">
          <img :src="work.photo" alt="" />
        </div>
      </div>
    </section>
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
<style lang="scss" scoped>
.card-list {
  display: flex;
  padding: 3rem;
  overflow-x: scroll;
  ::-webkit-scrollbar {
    width: 10px;
    height: 10px;
  }

  /* Track */
  ::-webkit-scrollbar-track {
    background: linear-gradient(
      90deg,
      #201c29,
      #201c29 1px,
      #17141d 0,
      #17141d
    );
  }

  /* Handle */
  ::-webkit-scrollbar-thumb {
    background: #201c29;
    border-radius: 10px;
    box-shadow: inset 2px 2px 2px hsla(0, 0%, 100%, 0.25),
      inset -2px -2px 2px hsla(0, 0%, 0%, 0.25);
  }
}

.card {
  display: flex;
  position: relative;
  flex-direction: column;
  height: 650px;
  width: 500px;
  min-width: 350px;
  padding: 1rem;
  border-radius: 16px;
  background: #17141d;
  box-shadow: -1rem 0 3rem #000;
  transition: 0.2s;

  &:hover {
    transform: translateY(-1rem);
  }
  &:hover ~ .card {
    transform: translateX(250px);
  }
  &:not(:first-child) {
    margin-left: -250px;
  }
  -webkit-animation: slide-in-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) ;
  animation: slide-in-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) ;
  .card-header,
  .card-img {
    width: 100%;
    //   max-width: 100%;
    img {
      width: 100%;
    }
  }
}
</style>
