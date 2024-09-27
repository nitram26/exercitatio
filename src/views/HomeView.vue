<template>
    <div>
      <Transition>
        <h1>ANIMACIONES en VUE3 COMPOSITION</h1>
      </Transition>
    </div>
    <v-btn>Mostrar</v-btn>
</template>
<!-- ************************************* -->
<script setup>

</script>
<!-- ************************************* -->
<style scoped>
.v-enter-from, .v-leave-to{
  opacity: 0;
}

.v-enter-active, .v-leave-active{
  transition: opacity 0.5s ease ;
}

.v-enter-to{

}

.v-leave-from{

}

</style> 