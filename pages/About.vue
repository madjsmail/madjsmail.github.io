<template>
  <div class="about">
    <div class="container">
      <section>
        <h2>
          A bit about myself
        </h2>
        <p>
          So, I’m <span class="upercase">madjid</span> — a Web dev and cs
          student in Algeria. I love everything that as to do with javascript ,
          web & open source, I don't stop learning, and I keep improving my self
          in all domains. and I like keeping it simple 😉 <br />
          <!-- I speak English, Arabic , franch & kabyle. -->
        </p>
      </section>
      <section class="section-list">
        <h2 class="section__header upercase">
          Skills
        </h2>
        <div class="section__content">
          <div class="line-card">
            <h5 class="line-card__header upercase">
              front end
            </h5>
            <div class="line-div line-card__content">
              <ul class="">
                <li
                  class="upercase"
                  v-for="(a, index) in frontend"
                  v-bind:key="index"
                >
                  <img
                    class="about-img"
                    :src="a.img"
                    :alt="a.name"
                    :style="
                      ` animation: slide-in-bottom 1s ease ${Math.random() *
                        0.8}s  both`
                    "
                  />
                  {{ a.name }}
                </li>
              </ul>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header upercase">
              back end
            </h5>
            <div class="line-div line-card__content">
              <ul>
                <li
                  class="upercase"
                  v-for="(a, index) in backend"
                  v-bind:key="index"
                >
                  <img
                    class="about-img"
                    :src="a.img"
                    :alt="a.name"
                    :style="
                      `
                  animation: slide-in-bottom 1s ease ${Math.random() * 1}s
                  both`
                    "
                  />
                  {{ a.name }}
                </li>
              </ul>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header upercase">
              database
            </h5>
            <div class="line-div line-card__content">
              <ul>
                <li
                  class="upercase"
                  v-for="(a, index) in database"
                  v-bind:key="index"
                >
                  <img
                    class="about-img"
                    :src="a.img"
                    :alt="a.name"
                    :style="
                      `
                  animation: slide-in-bottom 1s ease ${Math.random() * 1}s
                  both`
                    "
                  />
                  {{ a.name }}
                </li>
              </ul>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header upercase">
              UX UI
            </h5>
            <div class="line-div line-card__content">
              <ul>
                <li
                  class="upercase"
                  v-for="(a, index) in uxui"
                  v-bind:key="index"
                >
                  <img
                    class="about-img"
                    :src="a.img"
                    :alt="a.name"
                    :style="
                      `
                  animation: slide-in-bottom 1s ease ${Math.random() * 1}s
                  both`
                    "
                  />
                  {{ a.name }}
                </li>
              </ul>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header upercase">
              Other
            </h5>
            <div class="line-div line-card__content">
              <ul>
                <li
                  class="upercase"
                  v-for="(a, index) in other"
                  v-bind:key="index"
                >
                  <img
                    class="about-img"
                    :src="a.img"
                    :alt="a.name"
                    :style="
                      `
                  animation: slide-in-bottom 1s ease ${Math.random() * 1}s
                  both`
                    "
                  />
                  {{ a.name }}
                </li>
              </ul>
            </div>
          </div>
        </div>
      </section>
      <section class="section-list">
        <h2 class="section__header upercase">
          Cursus
        </h2>
        <div class="section__content">
          <div class="line-card">
            <h5 class="line-card__header">
              2012 - 2017
            </h5>
            <div class="line-div line-card__content">
              <h5 class="">
                High School
              </h5>
              <p>
                Scientific Baccalaureate
              </p>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header">
              2017 - 2020
            </h5>
            <div class="line-div line-card__content">
              <h5>
                University Uamob
              </h5>
              <p>
                Bachelor's Degree In Computer Science.
              </p>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header">
              2020 -
            </h5>
            <div class="line-div line-card__content">
              <h5>
                University Uamob
              </h5>
              <p>
                Master Degree In Computer Science.
              </p>
            </div>
          </div>
        </div>
      </section>
      <section class="section-list">
        <h2 class="section__header upercase">
          Experiences
        </h2>
        <div class="section__content">
          <div class="line-card">
            <h5 class="line-card__header">
              2019 - 2020
            </h5>
            <div class="line-div line-card__content">
              <h5 class="upercase">
                SETRAM
              </h5>
              <p>
                Web Developer
              </p>
            </div>
          </div>
          <div class="line-card">
            <h5 class="line-card__header">
              2020 -
            </h5>
            <div class="line-div line-card__content">
              <h5 class="upercase">
                Algerium
              </h5>
              <p>
                Web Developer
              </p>
            </div>
          </div>
        </div>
      </section>

      <section class="section-cards">
        <h3 class="section__header upercase">
          where i learned programming
        </h3>
        <div class="section__content">
          <div
            class="section__content__card flex-center"
            v-for="(a, index) in learning"
            v-bind:key="index"
          >
            <img class="" :src="a.img" :alt="a.name" srcset="" />
            <p>{{ a.name }}</p>
          </div>
        </div>
      </section>
      <section class="section-cards">
        <h3 class="section__header upercase">
          my favorite youtube channels
        </h3>
        <div class="section__content">
          <div
            class="section__content__card flex-center"
            v-for="(a, index) in youtube"
            v-bind:key="index"
          >
            <img class="" :src="a.img" :alt="a.name" srcset="" />

            <a href="">{{ a.name }}</a>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      frontend: [
        {
          name: "html",
          img: require("../assets/icons/skills/icons8-html-5-50.png")
        },
        {
          name: "css",
          img: require("../assets/icons/skills/icons8-css3-50.png")
        },
        {
          name: "scss",
          img: require("../assets/icons/skills/icons8-sass-50.png")
        },
        {
          name: "javascript",
          img: require("../assets/icons/skills/icons8-source-code-50.png")
        },
        {
          name: "vuejs",
          img: require("../assets/icons/skills/icons8-vuejs-50.png")
        },
        {
          name: "react",
          img: require("../assets/icons/skills/icons8-react-native-50.png")
        }
      ],
      backend: [
        {
          name: "php",
          img: require("../assets/icons/skills/icons8-php-logo-50.png")
        },
        {
          name: "laravel",
          img: require("../assets/icons/skills/icons8-laravel-50.png")
        },
        {
          name: "nodejs",
          img: require("../assets/icons/skills/icons8-nodejs-50.png")
        },
        {
          name: "EXPRESS",
          img: require("../assets/icons/skills/icons8-nodejs-50.png")
        }
      ],
      database: [
        {
          name: "firebase",
          img: require("../assets/icons/skills/icons8-source-code-50.png")
        },
        {
          name: "SQL",
          img: require("../assets/icons/skills/icons8-sql-50.png")
        }
      ],
      uxui: [
        {
          name: "adobe xd",
          img: require("../assets/icons/skills/icons8-adobe-xd-50.png")
        }
      ],
      other: [
        {
          name: "git/github",
          img: require("../assets/icons/skills/icons8-git-50.png")
        }
      ],
      learning: [
        {
          name: "youtube",
          img: require("../assets/icons/skills/youtube.png")
        },
        {
          name: "stackoverflow",
          img: require("../assets/icons/skills/stack.png")
        },
        {
          name: "udemy",
          img: require("../assets/icons/skills/udemy.png")
        },
        {
          name: "freecodecamp",
          img: require("../assets/icons/skills/freecodecamp.png")
        }
        //   {
        //   name: "Not school",
        //   img: require("../assets/icons/skills/freecodecamp.png"),
        // },
      ],
      youtube: [
        {
          name: "thenewboston",
          img: require("../assets/icons/skills/thenewboston.png")
        },
        {
          name: "fireship io",
          img: require("../assets/icons/skills/fireship.png")
        },
        {
          name: "traversy media",
          img: require("../assets/icons/skills/traversy.png")
        }
      ]
    };
  }
};
</script>
