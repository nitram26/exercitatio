<template>
  <h1>VUE3</h1>
    <div class="uno">
    
      <button @click="handleLayout(ListLayout)">LISTA</button>
      <button  @click="handleLayout(CardLayout)">TARJETA</button>
      <button  @click="handleLayout(TableLayout)">TABLA</button>
    </div>
    <component :is="layout" :content="users"/>
</template>
<!-- ************************************* -->
<script setup>
import { ref, defineAsyncComponent } from 'vue';


const ListLayout = defineAsyncComponent(()=> import('@/layouts/ListLayout.vue'))
const TableLayout= defineAsyncComponent(() => import('@/layouts/tableLayout.vue'))
const CardLayout= defineAsyncComponent(()=> import('@/layouts/CardLayout.vue'))

const layout = ref(ListLayout)
const handleLayout = (cmp) => layout.value = cmp


const users = ref([
  {
    name:'Carlos',
    age: 65,
    pocition: 'desarrollador'
  },
  {
    name:'Martin',
    age: 11,
    pocition: 'back'
  },
  {
    name:'Nestor',
    age: 22,
    pocition: 'front'
  },
  {
    name:'Jose',
    age: 33,
    pocition: 'bd'
  },
  {
    name:'Pedro',
    age: 44,
    pocition: 'analista'
  },
])
</script>
<!-- ************************************* -->
<style scoped>
.uno{
  display: flex;
}
.uno button{
  background-color: brown;
  color: aliceblue;
  margin: 1em;
}
</style>