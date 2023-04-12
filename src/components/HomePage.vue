<script setup lang="ts">
import Hero from './Hero.vue';
import WhatIDo from './WhatIDo.vue';
import IWork from './IWork.vue';
import MyPoject from './MyProject.vue';
import WorkTogether from '../Features/WorkTogether.vue';
import type { Page } from '@/Interfaces/type';


const props = defineProps<{
    page: Page
}>()
const emit = defineEmits<{
    (e: 'navigate', page : Page) : void ;
}>()

</script>

<template>

<Hero />
<WhatIDo/>
<MyPoject @navigate="emit('navigate', $event)" :page="props.page"/>
<WorkTogether/>
</template>

<style scoped lang="scss">
</style>
