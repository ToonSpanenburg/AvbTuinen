<script setup>
var fullTime = new Date();
const year = fullTime.getFullYear();
</script>

<template>
  <div class="d-flex flex-wrap justify-content-between align-items-center py-3 mt-5 border-top mx-5">
    <div class="col-md-4 d-flex align-items-center">
      <span class="mb-3 mb-md-0 text-muted">© {{year}} AvbTuinen</span>
    </div>
  </div>
</template>

<style scoped>
.border-top
{
  border-top: #d6c389;
}
</style>