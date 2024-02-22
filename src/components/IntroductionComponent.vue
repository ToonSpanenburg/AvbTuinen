<script setup>

</script>

<template>
  <div>
    <div class="BgImage"></div>
    <div class="content">
      <div class="container m-5 p-5">
        <h2 class="myText">
          Avb Tuinen
        </h2>
        <div class="mt-3 w-50 mb-auto">
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
  height: 95%;
  position: absolute;
  filter: blur(1px);
  z-index: -1;
}

.content {
  position: relative;
  z-index: 1;
  color: antiquewhite;
  padding: 40px;
}

h2
{
  font-size: 4em;
}
h3
{
  font-size: 2em;
}
p
{
  font-size: 1.4em;
}

</style>