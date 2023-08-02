<template>
  <Head title="HomePage" />

  <h1
    class="w-full text-center text-2xl text-teal-50 bg-cyan-500 hover:bg-cyan-600 focus:text-red-500"
  >
    Hello, {{ name }}, {{ framework }}
  </h1>

  <Nav />
</template>

<script >

import { Head } from "@inertiajs/vue3";

import Nav from "../Shared/Nav.vue";

export default {
  components: { Head, Nav },

  props: {
    name: String,
    framework: Array,
  },
};
</script>


<style>
</style>