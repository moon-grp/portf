<template>
  <v-app class="body">
    <transition name="router_animation" enter-active-class="animated slideInLeft" leave-active-class="animated fadeOutDown">
      <Nuxt />
    </transition>
    
  </v-app>
</template>

<script>
export default {
  data() {
    return {}
  }
}
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.2/animate.min.css");
.body {
  min-height: 100%;
  background-color: #05014a;
  margin: 0;
}
</style>
