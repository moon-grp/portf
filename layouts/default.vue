<template>
  <v-app class="body">
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
  background-color: #fff;
}
</style>