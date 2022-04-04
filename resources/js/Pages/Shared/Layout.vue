<template>
  <header>
    <Nav />
  </header>

  <section>
    <div class="container">
      <iframe
        src="https://www.listennotes.com/podcasts/the-laracasts-snippet-jeffrey-way-28_iuCrmB-Z/embed/"
        height="600px"
        width="100%"
        style="width: 1px; min-width: 100%"
        frameborder="0"
        scrolling="no"
        loading="lazy"
      ></iframe>
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
