<script>
  export default {
      name: 'AppMainContent'
  }
</script>

<template>
  <!-- https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0 -->

  <section class="cards-wrapper">
    <div class="container">
      <div class="cards-list">
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
        <div class="card">temporibus perspiciatis autem minus error aut nesciunt repudiandae adipisci enim incidunt odit nam, aspernatur voluptates obcaecati.</div>
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

      .card {
        width: calc(100% / 5);
        padding: 5px;
      }
    }
  }
}
</style>