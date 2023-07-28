<template>
  <header class="header-container container">
    <NavBar />
    <HeaderContents />
  </header>
</template>

<script setup>
import NavBar from "./NavBar.vue";
import HeaderContents from "./HeaderContents.vue";
</script>

<style scoped>
.header-container {
  padding: 1.25rem;
  margin-block-end: 3.75rem;
}

.header-container > * + * {
  margin-block-start: 5rem;
}

@media only screen and (min-width: 57.5rem) {
  .header-container > * + * {
    margin-block-start: 8rem;
  }

  .header-container {
    min-height: 100vh;

    padding: 2.5rem 0;
  }
}
</style>
