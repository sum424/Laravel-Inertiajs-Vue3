<template>
  <h1>Users</h1>

  <div class="bg-success" style="margin-top: 1800px">
    <p>The current Time is {{ time }}</p>
    <Link href="/users" preserve-scroll>Refresh</Link>
  </div>
</template>

<script setup>
import Layout from "./Shared/Layout.vue";
import { Link } from "@inertiajs/inertia-vue3";
// no needs to declare them as auto called after imported
Component({ Layout: Layout });

defineProps({
  time: String,
});
</script>
