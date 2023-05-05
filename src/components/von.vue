<template>
  <div>
    <input :value="text" v-on:input="converToUpperCase" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "test",
    };
  },
  methods: {
    converToUpperCase(event) {
      this.text = event.target.value.toUpperCase();
    },
  },
};
</script>