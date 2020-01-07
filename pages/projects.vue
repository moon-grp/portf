<template>
  <v-container>
    <v-row class="mt-9">
      <v-col v-for="card in cards" :key="card.title" :cols="card.flex">
        <v-card raised  max-width="344">
          <v-img
            :src="card.src"
            class="white--text align-end"
            height="150px"
          >
          </v-img>
          <v-card-title v-text="card.title"></v-card-title>
           <v-card-subtitle v-text="card.sub">
    
    </v-card-subtitle>
          <v-card-actions>
          

            <v-btn icon>
              <v-icon>mdi-github-circle</v-icon>
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn icon>
              <v-icon>mdi-link-variant</v-icon>
            </v-btn>

            
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'projects',
  data: () => ({
    cards: [
      { title: 'Expense Dashboard', src: '/expense.png', flex: 3, sub: "An Expense tracker built with vuejs and vuetify" },
      { title: 'BoroDash', src: '/borodash.png', flex: 3, sub:"A simple fintech dashboard for softloan" },
      { title: 'EmployeeDash', src: '/empdash.png', flex: 3, sub:"An employee internal communication dashboard built with vuejs, vuetify and github api" },
      { title: 'Coffe shop', src: '/coffee.png', flex: 3, sub:"landing page for coffe shop built with vuejs and vuetify" },
      { title: 'Qinsurance', src: '/insure.png', flex: 3, sub:"QInsurance dashboard built with vuejs and vuebootstrap" },
      { title: 'Reiner', src: '/reiner.png', flex: 3, sub:"Text translator built with vuejs, vuetify and yandex Api" },
      { title: 'Reiss', src: '/reiss.png', flex: 3, sub:"  Crypto currency dashboard built with quasar framework and cryptocompare api" }
    ]
  })
}
</script>

<style scoped>
.font {
  font-family: 'Dosis', sans-serif;
  font-size: 25px;
  color: #05014a;
}
</style>
