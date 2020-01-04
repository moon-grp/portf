<template>
  <v-container class="pt-12 px-auto">
    <v-row class="mt-12">
      <div class="font_nav">
        Experience
      </div>
    </v-row>
    <v-row class="mt-2">
      <div class="font_nav">
        Projects
      </div>
    </v-row>
    <v-row class="pusherT font_name">
      <div>
        Olumide Adebayo
      </div>
    </v-row>
    <v-row>
      <div class="font_style">
        Frontend developer with 2+ years of experience. <br />
        I create innovative, accessible and fast webapps using vuejs.
      </div>
    </v-row>
    <v-row class="pt-2 ml-n3">
      <v-btn href="http://github.com/moon-grp" tile x-large color="#ccc" text icon>
        <v-icon>mdi-github-circle</v-icon>
      </v-btn>
      <v-btn href="https://twitter.com/GrpMoon" tile x-large color="#ccc" text icon>
        <v-icon>mdi-twitter</v-icon>
      </v-btn>
      <v-btn href="https://www.linkedin.com/in/olumide-adebayo-263321158/" tile x-large color="#ccc" text icon>
        <v-icon>mdi-linkedin</v-icon>
      </v-btn>
    </v-row>
    <v-row class="pt-2"> 
      <v-btn x-large color="#BFFCF9" class="btnish">Send me a Message</v-btn>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'home'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Baloo+Bhai|Oswald:300,400&display=swap');
.font_nav {
  font-family: 'Oswald', sans-serif;
  font-size: 25px;
  color: #ec87e4;
}
.btnish{
  border-radius: .5em;
  box-shadow: -12px -12px 12px 0 rgba(255, 255, 255, 1),
  12px, 12px, 12px, 0 rgba(0, 0, 0, 1)
}
.font_name {
  font-family: 'Baloo Bhai', cursive;
  font-size: 47px;
  color: #ec87e4;
  font-weight: 400;
}

.pusherT {
  padding-top: 10%;
}

.font_style {
  font-family: 'Oswald', sans-serif;
  font-size: 20px;
  color: #ec87e4;
}

.btn_font {
  font-family: 'Oswald', sans-serif;
  font-size: 60px;
  font-weight: bold;
}
</style>
