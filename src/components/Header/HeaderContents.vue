<template>
  <section class="header__main header__spacing">
    <div class="header-main__img">
      <img src="../../assets/illustration-1.svg" alt="Intro Banner" />
    </div>

    <div class="header-main__textbox header__spacing">
      <h1 class="main__title">
        All your files in one secure location, accessible anywhere.
      </h1>

      <p class="base__font">
        Fylo stores your most important files in one secure location. Access
        them wherever you need, share and collaborate with friends, family, and
        co-workers.
      </p>

      <HeaderForm
        placeholder="Enter Your Email..."
        btnTitle="Get Started"
        btnClass="btn"
      />
    </div>
  </section>
</template>

<script setup>
import HeaderForm from "./HeaderForm.vue";
</script>

<style lang="scss" scoped>
.header__main {
  width: 100%;
}

.header__spacing > * + * {
  margin-block-start: 1.25rem;
}

:where(.header-main__img, .header-main__textbox) {
  --max-width: 26.25rem;
  width: min(100%, var(--max-width));
  margin-inline: auto;
}

.header-main__textbox {
  text-align: center;
}

@media only screen and (min-width: 57.5rem) {
  .header__main {
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
  }

  .header-main__img {
    --max-width: 40.625rem;
    margin-inline: 0;
  }

  .header__main .header-main__textbox {
    --max-width: 31.25rem;
    margin-inline: 0;

    text-align: left;
    margin-block-start: 4rem;

    & .main__title {
      line-height: 1.5;
    }
  }
}
</style>
