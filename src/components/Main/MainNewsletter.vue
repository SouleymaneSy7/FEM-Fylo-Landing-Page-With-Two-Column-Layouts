<template>
  <section class="newsletter">
    <section class="newsletter-container container spacing">
      <div class="newsletter__textbox spacing">
        <h2 class="title-2">Get early access today</h2>

        <p class="base__font">
          It only takes a minute to sign up and our free starter tier is
          extremely generous. If you have any questions, our support team would
          be happy to help you.
        </p>
      </div>

      <NewsletterForm
        placeholder="email@example.com"
        btnTitle="Get Started For Free"
        btnClass="btn btn2"
      />
    </section>
  </section>
</template>

<script setup>
// Imports
import NewsletterForm from "./NewsletterForm.vue";
</script>

<style lang="scss" scoped>
.newsletter {
  background-color: var(--secondary-clr);

  padding: 3.75rem 1.25rem;
}

.newsletter__textbox,
.form {
  --max-width: 26.25rem;
  width: min(100%, var(--max-width));

  text-align: center;

  margin-inline: auto;
}

:is(.newsletter .title-2, .newsletter .base__font) {
  color: var(--light-grayish-blue);
}

.spacing > * + * {
  margin-block-start: 1.25rem;
}

@media only screen and (min-width: 57.5rem) {
  .newsletter {
    padding: 5rem 0;
  }

  .newsletter-container {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
  }

  .newsletter__textbox {
    --max-width: 31.25rem;
    text-align: left;
    margin-inline: 0;
  }

  .newsletter-container.spacing > * + * {
    margin-block-start: 0;
  }

  .form {
    margin: 0;
    text-align: left;
  }
}
</style>
