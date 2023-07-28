<template>
  <form class="form" @submit.prevent="formSubmit">
    <label>
      <input
        type="email"
        class="input"
        :class="inputError == true ? 'errors' : ''"
        :placeholder="props.placeholder"
        v-model="inputValue"
        @input="formSubmit"
      />
      <span class="input__errors" v-if="inputError">
        {{ Errors }}
      </span>
    </label>

    <button type="submit" :class="btnClass">{{ props.btnTitle }}</button>
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
.form {
  display: flex;
  flex-direction: column;
  gap: 0.625rem;
}

:where(.input, .btn) {
  width: 100%;
}

@media only screen and (min-width: 57.5rem) {
  .form {
    gap: 1rem;
    text-align: left;
  }

  .input {
    width: 100%;
  }

  .btn.btn2 {
    width: fit-content;
    padding: 0.75rem 2rem;

    box-shadow: 0.125rem 0.1875rem 0.1875rem 0 hsl(var(--primary-clr-accent), 0.1);

    transition: opacity 200ms ease-in-out;
    cursor: pointer;

    &:is(:hover, :focus) {
      opacity: 0.9;
    }
  }
}
</style>
