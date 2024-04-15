<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppMainContent from "./components/AppMainContent.vue";

  export default {
    components: {
      AppHeader,
      AppMainContent
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
