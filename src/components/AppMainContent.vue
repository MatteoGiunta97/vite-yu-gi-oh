<script>
  import { store } from "../store.js";
  import Card from "./Card.vue";

  export default {
      name: 'AppMainContent',
        components: {
          Card
        }
        ,
        data() {
          return {
            store
          };
        }
  }
</script>

<template>
  
  <section class="cards-wrapper">
    <div class="container">
      <div class="cards-list">
        <Card v-for="card in store.cards" :key="card.id" :cardInfo="card"></Card>
      </div>
    </div>
  </section>

</template>

<style scoped lang="scss">

.cards-wrapper {
  background-color: #d48f38;
  padding: 20px;

  .container {
    background-color: white;

    .cards-list {
      display: flex;
      flex-wrap: wrap;
    }
  }
}
</style>