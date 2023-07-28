<template>
  <nav class="navbar">
    <a href="#" class="navbar__logo">
      <img src="../../assets/logo.svg" alt="Website Logo" />
    </a>

    <ul>
      <li v-for="(link, index) in headerLinks" :key="index">
        <a href="#" class="link"> {{ link }} </a>
      </li>
    </ul>
  </nav>
</template>

<script setup>
// Imports
import { ref } from "vue";

const headerLinks = ref(["Features", "Team", "Sign In"]);
</script>

<style lang="scss" scoped>
.navbar {
  width: 100%;

  display: flex;
  justify-content: space-between;
  align-items: center;

  & a.navbar__logo {
    width: 6.25rem;
    height: 1.875rem;

    & img {
      width: 100%;
      height: 100%;
    }
  }

  & ul li {
    display: inline-block;
    margin-inline-start: 0.75rem;
  }
}
</style>
