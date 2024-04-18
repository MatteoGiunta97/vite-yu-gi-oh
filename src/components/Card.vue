<script>
  export default {
      name: 'Card',
      props: {
        cardInfo: Object
      }
  }
</script>

<template>

    <div class="card">
        <div class="image">
            <img :src="cardInfo.card_images[0].image_url_small">
        </div>
        <div class="info-wrapper">
            <div class="name">
                <h3>{{ cardInfo.name }}</h3>
            </div>
            <div class="archetype">
                <h5>{{ cardInfo.archetype }}</h5>
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

        img {
            width: 100%;
        }
        
        .info-wrapper {
            background-color: #d48f38;
            text-align: center;
            padding: 10px;
            width: 100%;
            height: 100%;

            h3 {
                color:white;
            }
        }
      }

</style>