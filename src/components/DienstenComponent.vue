<script setup>
import {ref} from "vue";
import * as Diensten from "@/components/diensten/Diensten.js";
import IndividueleDienstComponent from "@/components/diensten/IndividueleDienstComponent.vue";

const alleDiensten = ref(Diensten.getAllDiensten());

</script>

<template>
  <div class="m-5 p-5">
    <div class="container DienstenPadding">
      <h2>
        Diensten
      </h2>
      <div class="mt-4">
        <div class="row">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi consectetur corporis, in iusto magnam molestiae officiis porro? Aliquam consequatur delectus doloribus impedit in magni, nesciunt nostrum odit officiis quis, soluta.
          </p>
          <div v-for="dienst in alleDiensten" class="col-3 mt-3">
            <IndividueleDienstComponent :Dienst="dienst"/>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<style scoped>
.DienstenPadding {
  padding-top: 30px;
  padding-left: 40px;
  padding-right: 40px;
}
h2{
  font-family: Baskerville Serif;
  font-size: 3em;
}
</style>