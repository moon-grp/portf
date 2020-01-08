<template>
  <v-container>
    <v-row class="mt-9">
      <v-col v-for="card in cards" :key="card.title" :cols="card.flex">
        <v-card raised max-width="344">
          <v-img :src="card.src" class="white--text align-end" height="150px">
          </v-img>

          <v-list-item three-line>
            <v-list-item-content>
              <v-list-item-title
                class="title"
                v-text="card.title"
              ></v-list-item-title>
              <v-list-item-subtitle v-text="card.sub"> </v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>

          <v-card-actions>
            <v-btn :href="card.github" icon>
              <v-icon>mdi-github-circle</v-icon>
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn :href="card.link" icon>
              <v-icon>mdi-link-variant</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    
    <v-btn
              dark
              fab
              top
              right
              color="pink"
            >
              <v-icon>mdi-plus</v-icon>
            </v-btn>
  </v-container>
</template>

<script>
export default {
  name: 'projects',
  data: () => ({
    cards: [
      {
        title: 'Expense Dashboard',
        src: '/expense.png',
        flex: 3,
        sub: 'An Expense tracker built with vuejs and vuetify.',
        github: 'https://github.com/moon-grp/fundall_exp',
        link: 'https://sandbox-expense.netlify.com'
      },
      {
        title: 'BoroDash',
        src: '/borodash.png',
        flex: 3,
        sub: 'A simple fintech dashboard for softloan.',
        github: 'https://github.com/moon-grp/borodash',
        link: 'https://boro-dash.netlify.com'
      },
      {
        title: 'EmployeeDash',
        src: '/empdash.png',
        flex: 3,
        sub:
          'An employee internal communication dashboard built with vuejs, vuetify and github api.',
        github: 'https://github.com/moon-grp/sandbox_employee_dashboard',
        link: 'https://sandbox-emp-dash.netlify.com'
      },
      {
        title: 'Coffe shop',
        src: '/coffee.png',
        flex: 3,
        sub: 'landing page for coffe shop built with vuejs and vuetify.',
        github: 'https://github.com/moon-grp/sandbox-prod-page',
        link: 'https://sandbox-coffee.netlify.com'
      },
      {
        title: 'Qinsurance',
        src: '/insure.png',
        flex: 3,
        sub: 'QInsurance dashboard built with vuejs and vuebootstrap.',
        github: 'https://github.com/moon-grp/natterbase_test',
        link: ''
      },
      {
        title: 'Reiner',
        src: '/reiner.png',
        flex: 3,
        sub: 'Text translator built with vuejs, vuetify and yandex api.',
        github: 'https://github.com/moon-grp/Project-reiner',
        link: 'https://project-reiner.netlify.com'
      },
      {
        title: 'Reiss',
        src: '/reiss.png',
        flex: 3,
        sub:
          '  Crypto currency dashboard built with quasar framework and cryptocompare api.',
        github: 'https://github.com/moon-grp/Project-Reiss',
        link: 'https://project-reiss.netlify.com'
      }
    ]
  })
}
</script>

<style scoped>

</style>
