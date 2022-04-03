<template>
  <header>
    <Nav />
  </header>

  <section>
    <div class="container">
      <slot />
    </div>
  </section>
</template>

<script>
import Nav from "./Nav.vue";

export default {
  components: { Nav },
};
</script>
