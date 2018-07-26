<template>
  <div id="app">
    <div class="container">
      <app-quote-grid :quotes="quotes"></app-quote-grid>
    </div>
  </div>
</template>

<script>
import QuoteGrid from "./components/QuoteGrid";
export default {
  name: "app",
  data: function() {
    return {
      quotes: ["Just a Quote"],
      maxQuotes: 10
    };
  },
  components: {
    appQuoteGrid: QuoteGrid
  }
};
</script>

<style>
</style>
