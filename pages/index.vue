<template>
  <section>
    <sec-header></sec-header>
    <sec-guideline :title="title" :bodyHtml="bodyHtml"></sec-guideline>
    <sec-footer></sec-footer>
  </section>
</template>

<script>
import secHeader from "~/components/pages/Top/Header.vue";
import secGuideline from "~/components/pages/Top/Guideline.vue";
import secFooter from "~/components/pages/Top/Footer.vue";

export default {
  components: {
    secHeader,
    secGuideline,
    secFooter
  },
    asyncData({ params }) {
      const obj = Object.assign({}, require(`../contents/posts/json/test.json`), { params });
      console.log(obj);
      return obj;
    },
    head() {
      const title = `${this.title} - logo-guideline`;
      const url = `https://logo-guideline.netlify.com/`;
      return {
        title: title,
        meta: [
          { hid: 'og:url', property: 'og:url', content: url },
          { hid: 'og:title', property: 'og:title', content: title },
        ],
        link: [{ rel: 'canonical', href: url }],
      };
    },
};
</script>

<style>
</style>
