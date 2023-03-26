<template>
  <MainPage />
</template>

<script>
import MainPage from "./page/MainPage.vue";

export default {
  name: "App",
  components: {
    MainPage,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  & {
    h1 {
      @apply text-5xl;
    }
    h2 {
      @apply text-4xl;
    }
    h3 {
      @apply text-3xl;
    }
    h4 {
      @apply text-2xl;
    }

    input {
      @apply py-2 px-4
      rounded
      mr-2;
      &[type="text"] {
        @apply shadow-lg  border-inherit;
      }
    }

    button {
      @apply rounded
      p-4 h-14;
    }
  }
}
</style>
