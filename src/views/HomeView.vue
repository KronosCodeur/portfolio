<template>
  <v-app>
    <nav-bar class="position-fixed "/>
    <v-container fluid style="background: #0A0E11">
      <div class="head d-flex justify-center align-center" id="home">
        <v-row>
          <v-col cols="6">
            <div class="mt-16 d-flex align-start justify-start flex-column" style="position: relative; ">
              <h2 class="text-green text-start" style="margin-left: 75px">SALUT, JE SUIS</h2>
              <h1 class="text-white text-start" style="font-size: 50px;margin-left: 75px">Sam Arris PIRALI</h1>
              <h3 class="text-green-accent-3 text-start" style="font-size: 20px;margin-left: 75px">Développeur Fullstack</h3>
              <h4 class="text-grey text-start" style="margin-left: 75px">
                Mes ambitions sont de mettre mes connaissances, compétences
                et expériences acquises au profit des entreprises pour une bonne productivité.😁
              </h4>
              <v-btn class="text-green-accent-4 mt-5" style="margin-left: 75px" dark title variant="outlined">Contactez-moi</v-btn>
              <div class="d-flex justify-start align-start flex-row" style="margin-left: 60px">
                <v-btn class="border-dashed icon mt-5 ml-3" icon="fa-brands fa-facebook" variant="outlined"/>
                <v-btn class="border-dashed icon mt-5 ml-3" icon="fa-brands fa-github" variant="outlined"/>
                <v-btn class="border-dashed icon mt-5 ml-3" icon="fa-brands fa-linkedin" variant="outlined"/>
              </div>
              <div class="d-flex justify-start align-start flex-row" style="margin-left: 60px">
                <v-btn class="border-dashed icon mt-5 ml-3" icon="fa-brands fa-x-twitter" variant="outlined"/>
                <v-btn class="border-dashed icon mt-5 ml-3" icon="fa-brands fa-instagram" variant="outlined"/>
                <v-btn class="border-dashed icon mt-5 ml-3" icon="fa-brands fa-telegram" variant="outlined"/>
              </div>
              <br/>
            </div>
          </v-col>
          <v-col cols="2">
            <div
                style="position:absolute; z-index: 10; bottom: -10vh ;margin-left: auto;margin-right: auto;left: 0; right:0; text-align: center">
              <a href="#about" class="text-white text-decoration-none"><v-icon>fas fa-angle-double-down</v-icon></a>
            </div>
          </v-col>
          <v-col cols="3">
            <div class="mt-16" style="position:relative; z-index: 10;">
              <image-viewer image-src="me.jpg" height="'450px'" message="Projets accomplis" width="'325px'" />
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col id="about" class="py-16 d-flex justify-center align-center " style="min-height: 100vh; border-bottom: 2px solid #01AF49 ;background: #0A0E11" cols="12">
        <div>
          <v-row>
            <v-col cols="12" sm="5">
              <div class="egg">
                <v-img class="bg-shades-transparent" contain max-height="300" src="me.png"></v-img>
              </div>
              <h1 class="text-center exp" style="font-size: 70px; color: red">2+</h1>
              <h1 class="text-center text-white" >Experience Technologique</h1>
            </v-col>
            <v-col cols="12" sm="7" class="pl-10">
              <h1 class="mt-16 text-uppercase ml-5" style="color: #01AF49">Qui suis-je?</h1><br/>
              <p class="mt-n4 ml-5" style="font-size: 30px; color: #FFF">Je suis un <span style="color: #01AF49; font-weight: bold">Dévéloppeur Fullstack</span> et passioné par le dévéloppement d'<span style="color: #01AF49; font-weight: 600">Application Mobile</span>.</p>
              <br/>
              <h3 class="ml-5" style="color: #01AF49">INFORMATIONS PERSONNELLES:</h3>
              <v-row>
                <v-col cols="6">
                  <v-list lines="lines" class="bg-transparent">
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Patronyme: PIRALI
                      </v-list-item-title>
                    </v-list-item>
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Address: Lomé,TOGO
                      </v-list-item-title>
                    </v-list-item>
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Telephone:
                        +22870097894
                      </v-list-item-title>
                    </v-list-item>
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Pays d'origine:
                        TOGO
                      </v-list-item-title>
                    </v-list-item>

                  </v-list>
                </v-col>
                <v-col class="text-left" cols="6">
                  <v-list lines="lines" class="bg-transparent">
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Prénoms: Sam Arris
                      </v-list-item-title>
                    </v-list-item>
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Email: arrispirali@gmail.com
                      </v-list-item-title>
                    </v-list-item>
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Loisirs:Jeux-Videos, Basketball</v-list-item-title>
                    </v-list-item>
                    <v-list-item prepend-icon="fa fa-circle-nodes" style="font-size: 13px; color: #01AF49">
                      <v-list-item-title style="font-size: 16px; font-weight: bold; color: #FFF">Freelance:
                        Disponible
                      </v-list-item-title>
                    </v-list-item>
                  </v-list>
                </v-col>
              </v-row>
              <v-btn class="mt-5 ml-10 py-2 px-3" style="color: white;font-weight: bold;font-size: medium; background: #01AF49; padding: 10px">Contactez-moi</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col id="services" class="py-16 px-12 d-flex align-center justify-space-between"  cols="12" style=" min-height: 100vh; background: #0A0E11; border-bottom: 2px solid #01AF49 ">
      </v-col>
      <v-col id="portfolio" class="py-16 px-12 d-flex align-center justify-space-between"  cols="12" style="min-height: 100vh; background: #0A0E11 ; border-bottom: 2px solid #01AF49 ">
        <v-col cols="6">
          <div>
            <h2 style="color: #01AF49; margin-bottom: 5px">Compétences</h2>
            <p class="text-white mb-6" style="font-size: 45px; font-weight: bold">Mes Compétences de prédilections.</p>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Flutter</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="90%" readonly="true" thumb-color="#01AF49" thumb-label="always" th thumb-size="0" />
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Symfony</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="85%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Kotlin</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="40%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Angular</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="60%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Git</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="80%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Adobe XD</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="85%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
        </v-col>
        <v-col cols="6">
          <p class="text-white font-weight-bold" style="font-size: 18px; margin-bottom: 50px; margin-top: 65px">J'apprends vite et m'adapte facilement. Lorsqu'un projet m'intéresse, j'ai de grandes capacités de travail, de concentration et d'innovation.</p>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Vue.js</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="65%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">ASP.Net</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="30%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Ktor</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="55%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Firebase</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="65%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Trello</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="85%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
          <div style="width: 90%">
            <h3 class="text-white ml-2">Jetbrains IDEs</h3>
            <v-slider class="flex-column" color="#01AF49" model-value="95%" readonly="true" thumb-label="always" th thumb-size="0"/>
          </div>
        </v-col>
      </v-col>
      <v-col id="contact" class="py-16 px-12 d-flex align-center justify-space-between"  cols="12" style="min-height: 100vh; background: #0A0E11">
      </v-col>
      <bottom-bar/>
    </v-container>
  </v-app>
</template>

<script>
import {defineComponent} from 'vue';

// Components
import NavBar from "@/components/NavBar.vue";

export default defineComponent({
  name: 'HomeView',
  data() {
    return {
      slider2: 50
    }
  },
  components: {
    NavBar,
  },
});
</script>
<style scoped>
.v-container {
  padding: 16px 0;
}

.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 80vh;
  width: 100%;
  background: #0A0E11;
  color: white;
}

.icon {
  border: 1px #01AF49;
  font-size: 15px;
}

.head:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: calc(100% + 10vh);
  width: 50%;
  background: #0A0E11;
  transform: skew(0, 6deg);
}

.head:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: calc(100% + 10vh);
  width: 50%;
  background: #0A0E11;
  transform: skew(0, -6deg);
}

.egg {
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #01AF49;
  box-shadow: 5px 5px 2px rgba(0, 0, 0, 0.03);
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
.exp:before{
  content: "2+";
  position: absolute;
  transform: translate(-2px);
  color: #01AF49;
}
.img{
  width: 100%;
  height: auto;
  border-radius: 5px 50px 5px 5px;
}
</style>
<script setup>
import ImageViewer from "@/components/ImageViewer.vue";
import BottomBar from "@/components/BottomBar.vue";
</script>