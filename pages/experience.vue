<template>
<div>
  <v-container>
    <v-row class="mt-9">
      <v-col lg="6" sm="12">
        <v-timeline dense>
          <v-timeline-item>
               <div>
          Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
        </div>
         <div>
          Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
        </div>
          </v-timeline-item>
          
          <v-timeline-item>
               <div>
          Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
        </div>
         <div>
          Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
        </div>
         <div>
          Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
        </div>
          </v-timeline-item>
        </v-timeline>
      </v-col>
      <v-col lg="6" sm="12"> this is for the skills </v-col>
    </v-row>
  </v-container>
   <v-bottom-navigation v-model="bottomNav" grow class="bg">
      <v-btn to="/" color="#ffe700" value="recent">
        <span>Home</span>
        <v-icon>mdi-home</v-icon>
      </v-btn>

      <v-btn to="/experience" color="#ffe700" value="experience">
        <span>Experience</span>
        <v-icon>mdi-office-building</v-icon>
      </v-btn>
    </v-bottom-navigation>
</div>
</template>

<script>
export default {
  name: 'experience',
  data: () => ({
    
})}
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
</style>
