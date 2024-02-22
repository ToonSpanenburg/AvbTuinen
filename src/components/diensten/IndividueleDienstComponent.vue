<script>
export default {
  props: ['Dienst']
};

</script>

<script setup>

</script>

<template>
  <div class="">
    <h3>
      {{Dienst.dienstNaam}}
    </h3>
    <div>
      {{Dienst.dienstText}}
    </div>
  </div>
</template>

<style scoped>

</style>