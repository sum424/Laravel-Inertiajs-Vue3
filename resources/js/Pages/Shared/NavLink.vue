<template>
  <Link :class="{ 'fw-bold text-white': active }">
    <slot />
  </Link>
</template>

<script>
import { Link } from "@inertiajs/inertia-vue3";
export default {
  components: { Link },
  props: {
    active: Boolean,
  },
};
</script>
