<template>
  <h1>Card</h1>
    <div class="container">
       <UserCard v-for="item in props.content" :key="item.name" :content="item"/>
    </div> 
</template>
<!-- ************************************* -->
<script setup>
import { defineProps } from 'vue';
import UserCard from '@/components/UserCard.vue'

const props = defineProps(['content'])
</script>
<!-- ************************************* -->
<style scoped>
.container{
  width: 100vw;
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  flex-wrap: wrap;
}
</style>