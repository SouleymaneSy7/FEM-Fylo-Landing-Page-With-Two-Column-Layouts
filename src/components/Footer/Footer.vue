<template>
  <footer class="footer">
    <section class="container spacing">
      <a href="#" class="footer__logo">
        <svg
          width="166"
          height="49"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
        >
          <defs>
            <path id="a" d="M.014.03h93.96v48.29H.015z" />
          </defs>
          <g fill="none" fill-rule="evenodd">
            <path
              class="square"
              d="M0 14.13v.123l27.95 13.13L56 14.209v-.033L27.95 1 0 14.13zm10.077.062L27.95 5.795l17.877 8.397-17.877 8.396-17.874-8.396zM27.95 32.483L0 19.55v4.784l27.95 12.964L56 24.289v-4.784L27.95 32.483zm0 9.703L0 29.25v4.783L27.95 47 56 33.99v-4.784l-28.05 12.98z"
            />
            <g transform="translate(72)">
              <mask id="b" fill="#fff">
                <use xlink:href="#a" />
              </mask>
              <path
                class="text"
                d="M87.56 24.152a8.1 8.1 0 0 0-2.161-5.573 7.259 7.259 0 0 0-2.34-1.673 6.864 6.864 0 0 0-2.85-.601c-1.01 0-1.961.2-2.852.601a7.257 7.257 0 0 0-2.34 1.673 8.102 8.102 0 0 0-2.16 5.574 8.102 8.102 0 0 0 2.16 5.573 7.257 7.257 0 0 0 2.34 1.672 6.864 6.864 0 0 0 2.851.602c1.01 0 1.96-.2 2.852-.602a7.259 7.259 0 0 0 2.339-1.672 8.1 8.1 0 0 0 2.16-5.574zm6.415 0c0 1.932-.357 3.723-1.07 5.373a13.098 13.098 0 0 1-2.94 4.28c-1.247 1.205-2.71 2.156-4.388 2.854-1.678.699-3.468 1.048-5.369 1.048-1.9 0-3.683-.349-5.346-1.048a13.863 13.863 0 0 1-4.366-2.876 13.351 13.351 0 0 1-2.94-4.302c-.713-1.65-1.07-3.426-1.07-5.329 0-1.873.364-3.634 1.092-5.284a13.92 13.92 0 0 1 2.962-4.325 13.671 13.671 0 0 1 4.367-2.898 13.552 13.552 0 0 1 5.301-1.048c1.901 0 3.69.35 5.369 1.048 1.678.698 3.14 1.65 4.388 2.854 1.248 1.204 2.228 2.638 2.94 4.302.713 1.665 1.07 3.449 1.07 5.351zM64.258 36.905a8.6 8.6 0 0 1-1.715.58c-.638.148-1.3.222-1.982.222a9.84 9.84 0 0 1-2.74-.379 6.003 6.003 0 0 1-2.295-1.226c-.653-.565-1.173-1.3-1.56-2.207-.385-.907-.578-2-.578-3.277V.029h6.549v29.474c0 1.07.215 1.806.646 2.207.43.401.943.602 1.537.602.742 0 1.455-.223 2.138-.669v5.262zM50.492 11.22L38.908 41.854c-.861 2.289-1.99 3.939-3.386 4.95-1.396 1.01-3.06 1.515-4.99 1.515-.297 0-.623-.022-.98-.066a7.352 7.352 0 0 1-1.025-.201l-2.138-5.975a8.486 8.486 0 0 0 1.56.557c.534.134 1.039.201 1.514.201 1.01 0 1.93-.23 2.762-.691.832-.46 1.47-1.315 1.916-2.564l.891-2.586-9.935-25.773h6.995l5.925 16.588 5.57-16.588h6.905zM23.538 7.342H6.786v8.294h16.529v5.618H6.785v15.784H.015V1.412h23.524v5.93z"
                mask="url(#b)"
              />
            </g>
          </g>
        </svg>
      </a>

      <section class="footer__flex spacing">
        <div class="footer__info">
          <div class="info">
            <div class="info__img">
              <img src="../../assets/icon-phone.svg" alt="Phone Icons" />
            </div>

            <p class="base__font">Phone: +1-543-123-4567</p>
          </div>

          <div class="info">
            <div class="info__img">
              <img src="../../assets/icon-email.svg" alt="Email Icons" />
            </div>

            <p class="base__font">example@fylo.com</p>
          </div>
        </div>

        <ul class="footer__navbar">
          <li v-for="(link, index) in linksGroup1" :key="index">
            <a href="#" class="link">{{ link }} </a>
          </li>
        </ul>

        <ul class="footer__navbar">
          <li v-for="(link, index) in linksGroup2" :key="index">
            <a href="#" class="link">{{ link }} </a>
          </li>
        </ul>

        <div class="social-icons">
          <!-- Facebook -->

          <a href="#" class="sci">
            <svg xmlns="http://www.w3.org/2000/svg">
              <path
                d="M18.896 0H1.104C.494 0 0 .494 0 1.104v17.793C0 19.506.494 20 1.104 20h9.58v-7.745H8.076V9.237h2.606V7.01c0-2.583 1.578-3.99 3.883-3.99 1.104 0 2.052.082 2.329.119v2.7h-1.598c-1.254 0-1.496.597-1.496 1.47v1.928h2.989l-.39 3.018h-2.6V20h5.098c.608 0 1.102-.494 1.102-1.104V1.104C20 .494 19.506 0 18.896 0z"
              />
            </svg>
          </a>

          <!-- Twitter -->
          <a href="#" class="sci">
            <svg xmlns="http://www.w3.org/2000/svg">
              <path
                d="M20.667 2.797a8.192 8.192 0 01-2.357.646 4.11 4.11 0 001.804-2.27 8.22 8.22 0 01-2.606.996A4.096 4.096 0 0014.513.873c-2.649 0-4.595 2.472-3.997 5.038a11.648 11.648 0 01-8.457-4.287 4.109 4.109 0 001.27 5.478A4.086 4.086 0 011.47 6.59c-.045 1.901 1.317 3.68 3.29 4.075a4.113 4.113 0 01-1.853.07 4.106 4.106 0 003.834 2.85 8.25 8.25 0 01-6.075 1.7 11.616 11.616 0 006.29 1.843c7.618 0 11.922-6.434 11.662-12.205a8.354 8.354 0 002.048-2.124z"
              />
            </svg>
          </a>

          <!-- Instagram -->
          <a href="#" class="sci">
            <svg xmlns="http://www.w3.org/2000/svg">
              <path
                d="M10.333 1.802c2.67 0 2.987.01 4.042.059 2.71.123 3.976 1.409 4.1 4.099.048 1.054.057 1.37.057 4.04 0 2.672-.01 2.988-.058 4.042-.124 2.687-1.386 3.975-4.099 4.099-1.055.048-1.37.058-4.042.058-2.67 0-2.986-.01-4.04-.058-2.717-.124-3.976-1.416-4.1-4.1-.048-1.054-.058-1.37-.058-4.041 0-2.67.01-2.986.058-4.04.124-2.69 1.387-3.977 4.1-4.1 1.054-.048 1.37-.058 4.04-.058zm0-1.802C7.618 0 7.278.012 6.211.06 2.579.227.56 2.242.394 5.877.345 6.944.334 7.284.334 10s.011 3.057.06 4.123c.166 3.632 2.181 5.65 5.816 5.817 1.068.048 1.408.06 4.123.06 2.716 0 3.057-.012 4.124-.06 3.628-.167 5.651-2.182 5.816-5.817.049-1.066.06-1.407.06-4.123s-.011-3.056-.06-4.122C20.11 2.249 18.093.228 14.458.06 13.39.01 13.049 0 10.333 0zm0 4.865a5.135 5.135 0 100 10.27 5.135 5.135 0 000-10.27zm0 8.468a3.333 3.333 0 110-6.666 3.333 3.333 0 010 6.666zm5.339-9.87a1.2 1.2 0 10-.001 2.4 1.2 1.2 0 000-2.4z"
              />
            </svg>
          </a>
        </div>
      </section>
    </section>

    <section class="attribution">
      <p>
        Challenge by
        <a href="https://www.frontendmentor.io?ref=challenge" target="_blank"
          >Frontend Mentor</a
        >
      </p>

      <p>
        Coded <span>&hearts;</span> by
        <a href="https://github.com/SouleymaneSy7" target="_blank"
          >Souleymane Sy</a
        >
      </p>
    </section>
  </footer>
</template>

<script setup>
// imports
import { ref } from "vue";

// Data
const linksGroup1 = ref(["About Us", "Jobs", "Press", "Blog"]);
const linksGroup2 = ref(["Contact Us", "Terms", "Privacy"]);
</script>

<style lang="scss">
.spacing > * + * {
  margin-block-start: 2.5rem;
}

.footer {
  background-color: var(--primary-clr);

  padding: 3.75rem 1.25rem;
}

.container {
  --max-width: 26.25rem;
}

:is(.footer__logo svg .square, .footer__logo svg .text) {
  fill: var(--white);
}

.footer__info {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.footer__info .info {
  display: flex;
  align-items: center;
  gap: 1rem;

  & .info__img {
    width: 1.125rem;
    height: 1.125rem;

    & img {
      width: 100%;
      height: 100%;
    }
  }

  & .base__font {
    color: var(--white);
  }
}

.footer__navbar li {
  margin-block-end: 0.75rem;

  & .link {
    color: var(--light-grayish-blue);

    transition: color 250ms ease-out;

    &:is(:hover, :focus) {
      color: var(--bright-blue);
    }
  }
}

.social-icons {
  display: flex;
  align-items: center;
  gap: 1.25rem;

  & .sci {
    width: 2.5rem;
    height: 2.5rem;

    display: grid;
    place-items: center;

    border: 0.0625rem solid var(--white);
    border-radius: 50%;

    transition: border 250ms ease-out;

    &:hover {
      border-color: var(--bright-blue);
    }

    &:hover path,
    &:focus path {
      fill: var(--bright-blue);
    }

    & svg {
      width: 1.25rem;
      height: 1.25rem;
    }

    & path {
      fill: var(--white);
      transition: fill 250ms ease-out;
    }
  }
}

.attribution {
  text-align: center;
  margin-block-start: 2rem;

  & p {
    font-size: 1rem;
    color: var(--white);
    line-height: 1;
    & span {
      font-size: 1.75rem;
      color: var(--bright-blue);
    }
  }

  & a {
    font-size: 1.25rem;
    color: var(--bright-blue);

    transition: text-decoration 200ms ease-in-out;

    &:is(:hover, :focus) {
      text-decoration: underline;
    }
  }
}

@media only screen and (min-width: 57.5rem) {
  .footer {
    padding: 5rem 0;
  }
  .footer__flex {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
  }

  .container {
    --max-width: 75rem;
  }

  .footer__flex.spacing > * + * {
    margin-block-start: 0;
  }
}
</style>
