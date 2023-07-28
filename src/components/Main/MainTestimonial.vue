<template>
  <section class="testimonial__card">
    <div class="testimonial__quotes">
      <img src="../../assets/icon-quotes.svg" alt="Quotes Icons" />
    </div>

    <div class="testimonial__textbox">
      <p class="base__font">
        Fylo has improved our team productivity by an order of magnitude. Since
        making the switch our team has become a well-oiled collaboration
        machine.
      </p>
    </div>

    <div class="testimonial__profile">
      <div class="profile__img">
        <img src="../../assets/avatar-testimonial.jpg" alt="Men Picture" />
      </div>

      <div class="profile__info">
        <h3 class="base__font">Kyle Burton</h3>
        <span>Founder & CEO, Huddle</span>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped>
.testimonial__card > * + * {
  margin-block-start: 0.75rem;
}

.testimonial__card {
  width: min(100%, 24.0625rem);

  border-radius: 0.25rem;

  background-color: var(--white);
  box-shadow: 0.125rem 0.1875rem 0.9375rem 0.125rem hsl(var(--primary-clr-accent), 0.1);

  padding: 1.875rem;
  margin: 2rem auto 0;

  & .testimonial__quotes {
    width: 0.875rem;
    height: 0.875rem;

    aspect-ratio: 1;
    object-fit: cover;
  }

  & .testimonial__textbox .base__font {
    --normal: 0.875rem;
    --sub-normal-1: 0.625rem;

    line-height: 1.6;
  }

  & .testimonial__profile {
    display: flex;
    align-items: center;
    gap: 0.75rem;

    & .profile__img {
      width: 2.5rem;
      height: 2.5rem;

      & img {
        width: 100%;
        height: 100%;

        aspect-ratio: 1;
        object-fit: cover;

        border-radius: 50%;
      }
    }

    & .profile__info {
      margin-block-start: 0.3125rem;
    }

    & .profile__info .base__font {
      --normal: var(--sub-normal-2);
      font-size: var(--normal);
      font-weight: var(--fw-700);
      line-height: 1;
    }

    & .profile__info span {
      --sub-normal-2: 0.8125rem;
      font-size: var(--sub-normal-2);
      line-height: 1;
    }
  }
}

@media only screen and (min-width: 57.5rem) {
  .testimonial__card {
    margin-inline: 0;
  }
}
</style>
