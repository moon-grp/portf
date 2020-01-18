<template>
<div>
  <v-container>
    <v-row class="mt-9">
      <v-col
        v-for="card in cards"
        :key="card.title"
        :lg="card.flex"
        :sm="card.sm"
        :md="card.md"
      >
        <v-card raised max-width="344" class=" mx-auto">
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
  name: 'projects',
  data: () => ({
     bottomNav: 'recent',
    cards: [
      {
        title: 'Expense Dashboard',
        src: '/expense.png',
        flex: 3,
        sub: 'An Expense tracker built with vuejs and vuetify.',
        github: 'https://github.com/moon-grp/fundall_exp',
        link: 'https://sandbox-expense.netlify.com',
        sm: '12',
        md: '6'
      },
      {
        title: 'BoroDash',
        src: '/borodash.png',
        flex: 3,
        sub: 'A simple fintech dashboard for softloan.',
        github: 'https://github.com/moon-grp/borodash',
        link: 'https://boro-dash.netlify.com',
        sm: '12',
        md: '6'
      },
      {
        title: 'EmployeeDash',
        src: '/empdash.png',
        flex: 3,
        sub:
          'An employee internal communication dashboard built with vuejs, vuetify and github api.',
        github: 'https://github.com/moon-grp/sandbox_employee_dashboard',
        link: 'https://sandbox-emp-dash.netlify.com',
        sm: '12',
        md: '6'
      },
      {
        title: 'Coffe shop',
        src: '/coffee.png',
        flex: 3,
        sub: 'landing page for coffe shop built with vuejs and vuetify.',
        github: 'https://github.com/moon-grp/sandbox-prod-page',
        link: 'https://sandbox-coffee.netlify.com',
        sm: '12',
        md: '6'
      },
      {
        title: 'Qinsurance',
        src: '/insure.png',
        flex: 3,
        sub: 'QInsurance dashboard built with vuejs and vuebootstrap.',
        github: 'https://github.com/moon-grp/natterbase_test',
        link: '',
        sm: '12',
        md: '6'
      },
      {
        title: 'Reiner',
        src: '/reiner.png',
        flex: 3,
        sub: 'Text translator built with vuejs, vuetify and yandex api.',
        github: 'https://github.com/moon-grp/Project-reiner',
        link: 'https://project-reiner.netlify.com',
        sm: '12',
        md: '6'
      },
      {
        title: 'Reiss',
        src: '/reiss.png',
        flex: 3,
        sub:
          '  Crypto currency dashboard built with quasar framework and cryptocompare api.',
        github: 'https://github.com/moon-grp/Project-Reiss',
        link: 'https://project-reiss.netlify.com',
        sm: '12',
        md: '6'
      },
       {
        title: 'Zaggadat',
        src: '/zagga.png',
        flex: 3,
        sub:
          'A sample PWA built with ionic4 and Vue.',
        github: 'https://github.com/moon-grp/ion',
        link: 'https://zaggadat.netlify.com',
        sm: '12',
        md: '6'
      }
    ],
     menu: [
       {
         title:'Home',
         to:"/"
       },
       {
         title:'Experience',
         to:"experience"
       },
        
      ],
  })
}
</script>

<style scoped>
.bg{
  background-color: #05014a;
}

.btn_font {
  font-family: 'Dosis', sans-serif;
  font-size: 15px;
  font-weight: bold;
  
}
</style>
