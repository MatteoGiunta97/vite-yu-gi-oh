<script>
  import axios from 'axios';
  import { store } from "./store.js";
  import AppHeader from "./components/AppHeader.vue";
  import AppMainContent from "./components/AppMainContent.vue";

  export default {
    components: {
      AppHeader,
      AppMainContent
    }
    ,
    data() {
      return {
        store
      };
    }
    ,
    methods: {
      getCardsFromApi() {
        
      }
    }
    ,
    mounted() {
      this.getCardsFromApi();
    }
  }
</script>

<template>
  <AppHeader></AppHeader>

  <main>
    <AppMainContent></AppMainContent>
  </main>
</template>

<style lang="scss">
  @use './style/generic';
</style>