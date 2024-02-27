<script setup>

</script>

<template>
  <div class="fullComponent p-3">
    <div class="container">
      <h1>
        Contact
      </h1>
      <div class="row">
        <div class="col-6">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ex magni repudiandae suscipit unde. Accusantium aperiam aut dicta impedit iure iusto labore laborum non, quaerat quidem sapiente, unde. Aliquam praesentium, vitae?
          </p>
          <ul class="ms-0 ps-0 ">

            <li class="mt-2 ">
              <a class="contactLink" href="tel:32471700000">
                <i class="bi bi-telephone-fill"></i>
                +32 471 70 00 00
              </a>
            </li>

            <li class="mt-2">
              <a class="contactLink" href="mailto: example@gmail.com">
                <i class="bi bi-envelope-fill"></i>
                example@gmail.com
              </a>
            </li>

          </ul>
          <div class="container-fluid" v-if="windowWidth > 1000">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d40225.96794994382!2d4.524728116251788!3d50.93993835237397!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47c3e08c3c1baa6b%3A0x40099ab2f4d5460!2s1910%20Kampenhout!5e0!3m2!1snl!2sbe!4v1708724318819!5m2!1snl!2sbe" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
          </div>
        </div>
        <div class="col-6  vraag rounded">
          <h2>
            Een vraag voor ons?
          </h2>
          <div class="mt-4">
            <form>
              <div class="form-group">
                <label for="uwNaam">Uw naam:</label>
                <input type="text" class="form-control" id="uwNaam" placeholder="peter paal">
              </div>

              <div class="form-group mt-2">
                <label for="uwEmail">Email address</label>
                <input type="email" class="form-control" id="uwEmail"  placeholder="uw mail">
              </div>

              <div class="form-group mt-2">
                <label for="uwBericht">Uw bericht:</label>
                <textarea class="form-control" id="uwBericht" rows="5"></textarea>
              </div>

              <button type="submit" class="btn btn-primary mt-3">Submit</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
    data() {
        return {
            windowWidth: window.innerWidth,
        };
    },
    mounted() {
        window.addEventListener('resize', this.handleResize);
    },
    beforeDestroy() {
        window.removeEventListener('resize', this.handleResize);
    },
    methods: {
        handleResize() {
            this.windowWidth = window.innerWidth;
        },
    },
};
</script>
<style scoped>
.fullComponent{
  //background-color: darkseagreen;
}
.vraag{
  //background-color: #8f7e14;
  //background-color: #004a22;
  //background-color: #4a671e;
}

a
{
  color: #8f7e14;
  text-decoration: none;
  font-size: 1.3em;
}
li
{
  list-style: none;
}
</style>