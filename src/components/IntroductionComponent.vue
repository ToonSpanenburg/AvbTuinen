<script setup>

import {getElement} from "bootstrap/js/src/util/index.js";
</script>

<template>
  <div class="">
    <div class="BgImage" id="BgImage">
      <div class="content">
        <div class="container p-5">
          <h2 class="myText">
            Avb Tuinen
          </h2>
          <div class= "my-5 row">
            <div class="col-12 col-sm-12 col-md-8 col-lg-6">
              <p class="myText">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquam aperiam consequatur, corporis illum ipsam necessitatibus quidem totam! Aut beatae, consequatur cupiditate eaque eius ipsam magnam minima numquam possimus quaerat qui.
              </p>
              <div class="mt-5">
                <h3 class="myText">
                  Subtitle
                </h3>
                <p class="myText">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo odio sint tempora voluptatum. Accusamus beatae ipsa quas quisquam quod ratione sint vel voluptate. Consequuntur deleniti doloribus earum explicabo, iure nam?
                </p>
              </div>
              <div class="mt-5">
                <h3 class="myText">
                  Subtitle
                </h3>
                <p class="myText">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo odio sint tempora voluptatum. Accusamus beatae ipsa quas quisquam quod ratione sint vel voluptate. Consequuntur deleniti doloribus earum explicabo, iure nam?
                </p>
              </div>
            </div>

          </div>
        </div>
      </div>
    </div>

  </div>
</template>


<style scoped>

.BgImage {
  background-image: url('/flower.jpg');
  background-size: cover;
  background-position: center;
  width: 100%;

}

img
{
  filter: blur(1px);
}

.content {
  position: relative;
  color: antiquewhite;
  padding: 40px;
}

h2
{
  font-size: 3em;
}
h3
{
  font-size: 2em;
}
p
{
  font-size: 1.4em;
}

@media (max-width: 1200px) {
    p
    {
        font-size: 1em;
    }
}
@media (min-width: 1200px) {
    p
    {
       font-size: 1.2em;
    }
}
</style>