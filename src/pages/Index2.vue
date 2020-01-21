<template>
  <div class="carousel-container">
    <div class="owl-carousel owl-theme owl-loaded">
      <carousel
        class="carousel"
        :autoplay="true"
        :loop="true"
        :nav="false"
        :center="true"
        :items="5 / 4"
        :mouseDrag="true"
      >
        <div class="gambar">
          <q-card class="kartumobil full-width">
            <img src="statics/mobil1.JPEG" />
          </q-card>
        </div>
        <div class="gambar">
          <q-card class="kartumobil full-width">
            <q-img src="statics/mobil1.JPEG">
              <div class="text-h5 absolute-bottom text-right">Title</div>
            </q-img>
          </q-card>
        </div>
        <div class="gambar">
          <q-card class="kartumobil full-width">
            <q-img src="statics/mobil1.JPEG">
              <div class="text-h5 absolute-bottom text-right">Title</div>
            </q-img>
          </q-card>
        </div>
        <div class="gambar">
          <q-card class="kartumobil full-width">
            <q-img src="statics/mobil1.JPEG">
              <div class="text-h5 absolute-bottom text-right">Title</div>
            </q-img>
          </q-card>
        </div>

        <div class="gambar">
          <q-card class="kartumobil full-width">
            <q-img src="statics/mobil1.JPEG">
              <div class="text-h5 absolute-bottom text-right">Title</div>
            </q-img>
          </q-card>
        </div>
        <div class="owl-dots">
          <div class="owl-dot active"><span></span></div>
          <div class="owl-dot"><span></span></div>
          <div class="owl-dot"><span></span></div>
        </div>
      </carousel>
    </div>
  </div>
</template>

<script>
import carousel from "vue-owl-carousel2";

export default {
  components: { carousel }
};
</script>

<style scoped>
.owl-item > div {
  cursor: pointer;
  margin: 6% 8%;
  transition: margin 0.4s ease;
}
.owl-item.center > div {
  cursor: auto;
  margin: 0;
}
.owl-item:not(.center) > div:hover {
  opacity: 0.75;
}
.carousel-container {
  padding-top: 20px;
}
.owl-theme .owl-dots .owl-dot span {
  max-width: 100%;
  background: gold;
  width: 10px;
  margin-top: -320%;
  position: relative;
  z-index: 999;
  text-align: center;
  margin-left: 2px;
  margin-right: 2px;
  display: block;

  transition: opacity 0.4s ease-in-out;
}
.owl-theme .owl-dots .owl-dot.active span {
  background: red;
  max-width: 100%;
  width: 15px;
  margin-top: -150%;
  opacity: 1;
  border-radius: 20px;
}
</style>
