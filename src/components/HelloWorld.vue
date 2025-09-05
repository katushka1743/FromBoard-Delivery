<script setup>
import benefits from './benefits.vue';
import garanty from './garanty.vue';
import headeVue from './header.vue';
import heroVue from './hero.vue';
import reviews from './reviews.vue';
import contactsForm from './contactsForm.vue';
import footerVue from './footer.vue';


</script>

<template>
  <heade-vue></heade-vue>
  <body>
    <hero-vue>
    </hero-vue>
    <benefits></benefits>
    <garanty></garanty>
    <reviews></reviews>
    <contactsForm></contactsForm>
  </body>

  <footerVue class="foot"></footerVue>
</template>

<style scoped>
body {
  background-color: #E5E7EB;
  width: 100dvw;
  padding: 0;
  margin: 0;
  padding-bottom: 72px;
}



</style>
