<template>
  <Layout>
    <h1>Users</h1>

    <div class="bg-success" style="margin-top: 1800px">
      <p>The current Time is {{ time }}</p>
      <Link href="/users" preserve-scroll>Refresh</Link>
    </div>
  </Layout>
</template>

<script>
import Layout from "./Shared/Layout.vue";
import { Link } from "@inertiajs/inertia-vue3";
export default {
  components: { Layout, Link },
  props: { time: String },
};
</script>
