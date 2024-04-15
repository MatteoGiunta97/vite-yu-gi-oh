<script>
  export default {
      name: 'Card'
  }
</script>

<template>

    <div class="card">
        <div class="image">
            <img src="#">
        </div>
        <div class="info-wrapper">
            <div class="name">
                <h3>test</h3>
            </div>
            <div class="type">
                <h5>test</h5>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">

.card {
        width: calc(100% / 5);
        padding: 10px;
        display: flex;
        align-items: center;
        flex-direction: column;
        
        .info-wrapper {
            background-color: #d48f38;
            text-align: center;
            padding: 10px;

            h3 {
                color:white;
            }
        }
      }

</style>