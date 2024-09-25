<template>
  <div class="list">
      <h1>UseList</h1>
      <h3>{{ props.content.name  }}</h3>
      <h3>Edad: {{ props.content.age }}</h3>
      <h3>{{ props.content.pocition }}</h3>
      <p></p>
  </div>
</template>
<!-- ************************************* -->
<script setup>
import { defineProps } from 'vue';

const props = defineProps(['content'])
</script>
<!-- ************************************* -->
<style scoped>
.list{
background-color: aquamarine;
border-radius: 10px;
padding: 10px;
display: flex;
justify-content: space-around;
width: 100%;
margin: 1em;
}
</style>