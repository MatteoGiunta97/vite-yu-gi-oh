<script>
  import Card from "./Card.vue";

  export default {
      name: 'AppMainContent',
        components: {
          Card
        }
  }
</script>

<template>
  
  <section class="cards-wrapper">
    <div class="container">
      <div class="cards-list">
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
        <Card></Card>
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