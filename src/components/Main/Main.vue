<template>
  <img
    src="../../assets/bg-curve-desktop.svg"
    class="bg-curve"
    alt="BG Curve"
  />
  <main class="main">
    <section class="main-container container">
      <section class="main__img">
        <img src="../../assets/illustration-2.svg" alt="" />
      </section>

      <section class="main__description">
        <h2 class="title-2">Stay productive, wherever you are</h2>

        <p class="base__font">
          Never let location be an issue when accessing your files. Fylo has you
          covered for all of your file storage needs.
        </p>

        <p class="base__font">
          Securely share files and folders with friends, family and colleagues
          for live collaboration. No email attachments required!
        </p>

        <div class="description__link">
          <span>See how Fylo works</span>

          <div>
            <img src="../../assets/icon-arrow.svg" alt="Arrow Icons" />
          </div>
        </div>

        <MainTestimonial />
      </section>
    </section>
  </main>

  <MainNewsletter />
</template>

<script setup>
// Imports
import MainTestimonial from "./MainTestimonial.vue";
import MainNewsletter from "./MainNewsletter.vue";
</script>

<style lang="scss" scoped>
.main {
  position: relative;
  padding: 3.75rem 1.25rem;

  background-color: var(--light-grayish-blue);
}

.main-container > * + * {
  margin-block-start: 3.75rem;
}

:where(.main__img, .main__description) {
  --max-width: 26.25rem;
  width: min(100%, var(--max-width));

  margin-inline: auto;
}

.main__description > * + * {
  margin-block-start: 1.25rem;
}

.main__description .title-2 {
  text-align: center;
}

.main__description .description__link {
  margin-inline: auto;
}

@media only screen and (min-width: 57.5rem) {
  .main {
    padding: 5rem 0;
  }

  .main-container {
    display: flex;
    flex-direction: row-reverse;
    align-items: flex-start;
    justify-content: space-between;
  }

  .main__img {
    --max-width: 34.375rem;

    margin-inline: 0;
  }

  .main__description {
    --max-width: 30rem;
    margin-inline: 0;

    & .title-2 {
      text-align: left;
    }

    & .description__link {
      margin-inline: 0;
    }
  }

  .main-container > * + * {
    margin-block-start: 0;
  }
}
</style>
