<template>
    <div class="row">
      <app-quote v-for="quote in quotes" :key="quote">{{quote}}</app-quote>
    </div>
</template>

<script>
import Quote from "../components/Quote.vue";

export default {
  props: ["quotes"],
  components: {
    appQuote: Quote
  }
};
</script>

<style>
</style>
