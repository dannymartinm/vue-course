<template>
    <div class="row">
      <form >
        <div class="col-sm-8 col-sm-offset-2 col-xs-12 col-md-6 col-md-offset-3 form-group">
          <label>Quote</label>
          <textarea class="form-control" rows="3" v-model="quote"></textarea>
        </div>
        <div class="col-sm-8 col-sm-offset-2 col-xs-12 col-md-6 col-md-offset-3 form-group">
          <button class="btn btn-primary" @click.prevent="createNew">
            Add Quote
          </button>
        </div>
      </form>
    </div>
</template>

<script>
export default {
  data() {
    return {
      quote: ""
    };
  },
  methods: {
    createNew() {
      //$emit() :Trigger an event on the current instance.
      //Any additional arguments will be passed into the listener’s callback function.
      this.$emit("quoteAdded", this.quote);
      this.quote = "";
    }
  }
};
</script>

<style>
</style>
