<template>
  <section>
    <sec-home></sec-home>
    <sec-footer></sec-footer>
  </section>
</template>

<script>
import secHome from "~/components/pages/Top/Home.vue";
import secFooter from "~/components/Footer.vue";

export default {
  components: {
    secHome,
    secFooter
  }
};
</script>

<style>
</style>
