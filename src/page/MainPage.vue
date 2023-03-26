<script setup>
// import { get } from "http";
import { ref } from "vue";
// import { IMaskComponent as imaskInput } from "vue-imask";
// const { mask } = imaskInput;

// const result = await fetch("https://jsonplaceholder.typicode.com/users");
// const json = await result.json();

const input = ref("");
</script>

<template>
  <div class="page">
    <!--<imask-input
    mask="+{7}(000)000-00-00"
    placeholder="imask"
    :value="inputValue"
    @input="inputValue = $event.target.value"
  />-->
    <div class="container">
      <h1 class="container__title">TODO LIST</h1>
      <div class="container__list">
        <input type="text" id="katakana" v-model="input" />
        <button>submit</button>
      </div>
      {{ input }}
    </div>
  </div>
</template>

<style scoped lang="scss">
button {
  @apply bg-amber-500 hover:bg-amber-400 hover:translate-x-1 hover:translate-y-1 hover:duration-100 duration-150 shadow-lg hover:shadow-md hover:shadow-amber-700/50 shadow-amber-600/50 text-white inline-block;
}
input[type="text"] {
  @apply w-5/6 h-14 border-sky-200 border shadow-sky-200/50 shadow-lg inline-block;
}
.container {
  @apply py-14 w-1/2 mx-auto h-full;
  &__title {
    @apply text-sky-800 py-10;
  }
  &__list {
    @apply py-10;
  }
}
.page {
  @apply w-full
  h-screen
  bg-sky-300;
}
</style>
