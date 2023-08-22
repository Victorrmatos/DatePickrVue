<template>
  <div class="box">
    <h1>Flatpickr + Vue 3</h1>
    <flat-pickr v-model="date" :config="config" />
    <hr />
    v-model: {{ date }}
  </div>
</template>

<script>
import flatPickr from "vue-flatpickr-component";
import "flatpickr/dist/flatpickr.css";

export default {
  data() {
    return {
      date: null,
      config: {
        inline: true,
      },
    };
  },
  components: {
    flatPickr,
  },
};
</script>

<style>
body {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>
