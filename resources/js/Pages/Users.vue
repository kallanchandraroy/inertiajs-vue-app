<template>
  <h1
    class="w-full text-center text-2xl text-teal-50 bg-cyan-500 hover:bg-cyan-600 focus:text-red-500"
  >
    Users
  </h1>
  <Nav />

  <div style="margin-top: 600px">
    <p>The current time is {{ time }}.</p>
    <Link href="/users" class="text-black" preserve-scroll>Refresh</Link>
  </div>
</template>

<script >
import { Head, Link } from "@inertiajs/vue3";

import Nav from "../Shared/Nav.vue";

export default {
  components: { Head, Nav, Link },

  props: {
    time: String,
  },
};
</script>


<style>
</style>