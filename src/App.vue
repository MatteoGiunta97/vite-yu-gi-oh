<script>
  import axios from 'axios';
  import { store } from "./store.js";
  import AppHeader from "./components/AppHeader.vue";
  import AppMainContent from "./components/AppMainContent.vue";
  import Search from './components/Search.vue';

  export default {
    components: {
      AppHeader,
      AppMainContent,
      Search
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
        
        const queryParams = {
          num: 20,
          offset: 0
        };

        if(store.selectedArchetype !== '') {
          queryParams.archetype = store.selectedArchetype
        };

        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php', {
          params: queryParams
        })
        .then((response) => {
          store.cards = response.data.data;
        });
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
    <Search @selectedSearch="getCardsFromApi"></Search>
    <AppMainContent></AppMainContent>
  </main>
</template>

<style lang="scss">
  @use './style/generic';
</style>