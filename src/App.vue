<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name: 'app',
    /*data () {
      return {
          showLogin: 0
      }
    },*/
    computed: {
      showLogin () {
          return this.$route.path === '/login' ? 1 : 0
      }
    },
    /*mounted() {
      if(this.$route.path === '/login'){
          this.showLogin = 1;
      } else {
        this.showLogin = 0;
      }
    },*/
    components: {

    }
  }
</script>

<style>

</style>
