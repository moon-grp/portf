<template>
  <div>
    <v-container>
      <v-row class="mt-9">
        <v-col lg="6" sm="12">
          <v-timeline class=" mx-auto" dense>
            <v-timeline-item small color="#ffe700">
              <h2 class="text">Frontend Developer</h2>
              <h5 class="mb-4 text_title">Davetechk, Abuja (2019 - Present)</h5>
              <div class="text_title">
                <div>- Develop new frontend features.</div>
                <div>- Small scale custom development for clients.</div>
                <div>- Client support.</div>
                <div>- Api integration.</div>
              </div>
            </v-timeline-item>

            <v-timeline-item small color="#ffe700">
              <h2 class="text">Frontend Developer</h2>
              <h5 class="mb-4 text_title">
                Insight Africa, Abuja (July 2018 - November 2018)
              </h5>
              <div class="text_title">
                <div>- Develop new frontend features.</div>
                <div>- Assisted in building studylab.</div>
                <div>- Api intergration</div>
              </div>
            </v-timeline-item>

            <v-timeline-item small color="#ffe700">
              <h2 class="text">Software Developer</h2>
              <h5 class="mb-4 text_title">
                Aiivon Innovations, Abuja (June 2017 - December 2017)
              </h5>
              <div class="text_title">
                <div>
                  - Worked on a school management webapp powered by electron.
                </div>
                <div>
                  - Built the android version of OneUrl; a social media card
                  app.
                </div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-col>
        <v-col lg="6" sm="12"> </v-col>
      </v-row>
    </v-container>
    <v-footer padless>
       <v-card
        flat
        tile
        width="100%"
        class="bg text-center"
      >
       <v-card-text>
          <v-btn
            v-for="menu in menu"
            :key="menu.title"
            class="mx-4 btn_font"
            color="#ccc"
            :to="menu.to"
            depressed
            outlined
          >
          <span v-text="menu.title"></span>
          </v-btn>
        </v-card-text>
       </v-card>
    </v-footer>
  </div>
</template>

<script>
export default {
  name: 'experience',
  data: () => ({
    bottomNav: 'recent',
     menu: [
       {
         title:'Home',
         to:"/"
       },
       {
         title:'Projects',
         to:"projects"
       },
        
      ],
  })
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Dosis:400,500&display=swap');
.text {
  color: #ffe700;
  font-family: 'Dosis', sans-serif;
}

.text_title {
  color: #ccc;
  font-family: 'Dosis', sans-serif;
}

.bg {
  background-color: #05014a;
}

.btn_font {
  font-family: 'Dosis', sans-serif;
  font-size: 15px;
  font-weight: bold;
  
}
</style>
