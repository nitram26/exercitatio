<template>
  <div class="row">
      <h1>UseRow</h1>
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
.row{
background-color: antiquewhite;
border-radius: 10px;
border: 1px brown solid;
padding: 10px;
display: flex;
flex-direction: column;
width: 12em;
margin: 1em;
}
</style>