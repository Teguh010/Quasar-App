<template>
  <q-layout>
    <div class="carousel-container">
      <div class="owl-carousel owl-theme owl-loaded">
        <carousel
          :autoplay="true"
          :loop="true"
          :nav="false"
          :center="true"
          :items="5 / 4"
          :mouseDrag="true"
          :dots="true"
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
        </carousel>
      </div>
    </div>
  </q-layout>
</template>

<script>
import carousel from "vue-owl-carousel2";

export default {
  components: { carousel }
};
</script>

<style lang="scss"  >
.owl-item > div {
  cursor: pointer;
  margin: 3% 3%;
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
  background: gold;
  height: 5px;
  width: 15px;
  margin: 2px;
}
.owl-theme .owl-dots {
  // margin-left: -130px;
  text-align: left;
  padding-left: 40px;
}

.owl-theme .owl-dots .owl-dot.active span {
  background: red;
  opacity: 1;
  transition: opacity 0.4s ease-in-out,
    width 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);

  width: 25px;
}
</style>
