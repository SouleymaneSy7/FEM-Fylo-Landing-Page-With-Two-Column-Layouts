<template>
  <form class="header__form" @submit.prevent="formSubmit">
    <label>
      <input
        type="email"
        class="input__outline"
        :class="inputError == true ? 'errors' : ''"
        :placeholder="props.placeholder"
        @input="formSubmit"
        v-model="inputValue"
      />
      <span class="input__errors" v-if="inputError">
        {{ Errors }}
      </span>
    </label>

    <button type="submit" :class="btnClass">
      {{ props.btnTitle }}
    </button>
  </form>
</template>

<script setup>
// Imports
import { ref } from "vue";

// Props
const props = defineProps({
  placeholder: String,
  btnTitle: String,
  btnClass: String,
  required: true,
});

// Variables
const Errors = ref("Please Check Your Email");
const inputValue = ref("");
const inputError = ref(false);
const regEx = /^([a-z\d\.-]+)@([a-z\d-]+)\.([a-z]{2,8})(\.[a-z]{2,8})?$/;

// Functions
const formSubmit = () => {
  if (regEx.test(inputValue.value)) {
    inputError.value = false;
  } else {
    inputError.value = true;
  }
};
</script>

<style lang="scss" scoped>
.header__form {
  display: flex;
  flex-direction: column;
  gap: 0.625rem;
}

:where(.input__outline, .btn) {
  width: 100%;
}

@media only screen and (min-width: 57.5rem) {
  .header__form {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;

    & label {
      flex-grow: 1;
    }
  }

  .btn {
    width: fit-content;
    height: fit-content;
  }

  .input__outline {
    width: 100%;
    flex-grow: 1;
  }
}
</style>
