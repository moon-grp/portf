<template>
  <v-container class="pt-12 px-auto">
    <v-row>
    <v-col cols="6">
      <v-row class="mt-6">
        <nuxt-link to="/">
          <div class="font_nav fancy-link">
            Experience & skills
          </div>
        </nuxt-link>
      </v-row>
      <v-row class="mt-2">
        <nuxt-link to="/projects">
          <div class="font_nav fancy-link">
            Projects
          </div>
        </nuxt-link>
      </v-row>
      <v-row class="pusherT font_name">
        <div>
          Olumide Adebayo.
        </div>
      </v-row>
      <v-row>
        <div class="font_style">
          Frontend developer with 2+ years of experience. <br />
          I create innovative, accessible and fast webapps using vuejs.
        </div>
      </v-row>
      <v-row class="pt-2 ml-n3">
        <v-btn
          href="http://github.com/moon-grp"
          tile
          x-large
          color="#ccc"
          text
          icon
        >
          <v-icon>mdi-github-circle</v-icon>
        </v-btn>
        <v-btn
          href="https://twitter.com/GrpMoon"
          tile
          x-large
          color="#ccc"
          text
          icon
        >
          <v-icon>mdi-twitter</v-icon>
        </v-btn>
        <v-btn
          href="https://www.linkedin.com/in/olumide-adebayo-263321158/"
          tile
          x-large
          color="#ccc"
          text
          icon
        >
          <v-icon>mdi-linkedin</v-icon>
        </v-btn>
      </v-row>
      <v-row class="pt-2">
        <v-btn x-large color="#ffe700" class="btn_font" depressed :href="`mailto:olumidemm@gmail.com`"
          >Send me a Message</v-btn
        >
      </v-row>
    </v-col>
    
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'home'
}
</script>

<style>
/*@import url('https://fonts.googleapis.com/css?family=Baloo+Bhai|Oswald:300,400&display=swap');   font-family: 'Baloo Bhai', cursive;*/
@import url('https://fonts.googleapis.com/css?family=Dosis:400,500&display=swap');
.font_nav {
  font-family: 'Dosis', sans-serif;
  font-size: 25px;
  color: #ffe700;
}

a {
  text-decoration: none;
}

.fancy-link {
  text-decoration: none;
  background-image: linear-gradient(#ccc, #ccc);
  background-repeat: no-repeat;
  background-position: bottom left;
  background-size: 0% 3px;
  transition: background-size 500ms ease-in-out;

  font-weight: var(--fw-bold);
}

.fancy-link:hover {
  background-size: 100% 3px;
  color: inherit;
}

.font_name {
  font-family: 'Dosis', sans-serif;
  font-size: 47px;
  color: #ffe700;
  font-weight: 400;
}

.pusherT {
  padding-top: 20%;
}

.font_style {
  font-family: 'Dosis', sans-serif;
  font-size: 20px;
  color: #ffe700;
}

.btn_font {
  font-family: 'Dosis', sans-serif;
  font-size: 60px;
  font-weight: bold;
}
</style>
