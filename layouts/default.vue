<template>
  <v-app class="body btnish">
  <Nuxt/>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>


<style scoped>
.body {
  min-height: 100vh;
  border-style: double;
  border-color: #bffcf9;
  border-width:5px;
  background-color: #FFFFFF;
}

.btnish{
  border-radius: .5em;
  box-shadow: -12px -12px 12px 0 rgba(255, 255, 255, 1),
  12px, 12px, 12px, 0 rgba(0, 0, 0, 1)
}
</style>