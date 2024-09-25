<template>
    <div class="card">
        <h1>UseCard</h1>
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
.card{
  background-color: aquamarine;
  border-radius: 10px;
  padding: 10px;
  display: flex;
  flex-direction: column;
  width: 12em;
  margin: 1em;
}
</style>