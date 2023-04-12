<script setup lang="ts">
import HomePage from './components/HomePage.vue';
import AboutMe from'./components/AboutMe.vue';
import BoutiqueProject from './components/BoutiqueProject.vue';
import { reactive, type Component as C } from 'vue';
import type { Page } from './Interfaces/type';
import TheFooter from './Features/Footer.vue'
import TheHeader from './Features/Header.vue'

const state = reactive<{
  page: Page,
}>({
  page: 'HomePage'
})

const pages: {[s:string] : C } = {
  HomePage,
  AboutMe,
  BoutiqueProject
}

function navigate (page: Page) : void {
  state.page = page;

  window.scrollTo({
    top: 0,
    left: 0
  })
}

</script>

<template>

<TheHeader 
@navigate="navigate" :page="state.page"
class="header"/>

<component :is="pages[state.page]"
@navigate="navigate" :page="state.page"
class="page"
 />

<TheFooter/>
</template>

<style scoped lang="scss">

.header {
    position: absolute;
    z-index: 2;
  }

  .page {
    position: relative;
    z-index: 1;
  }

</style>
