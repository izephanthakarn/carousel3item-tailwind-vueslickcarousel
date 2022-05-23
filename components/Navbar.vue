<template>
  <div class="mycontainer">
    <VueSlickCarousel class="bg-stone-900 container mycarousel" v-bind="settings">
      <div class="card">
        <div class="bg-carou">
          <div class="content">
            <h1 class="text-stone-100 text-6xl">1</h1>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="bg-carou">
          <div class="content">
            <h1 class="text-stone-100 text-6xl">2</h1>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="bg-carou">
          <div class="content">
            <h1 class="text-stone-100 text-6xl">3</h1>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="bg-carou">
          <div class="content">
            <h1 class="text-stone-100 text-6xl">4</h1>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="bg-carou">
          <div class="content">
            <h1 class="text-stone-100 text-6xl">5</h1>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="bg-carou">
          <div class="content">
            <h1 class="text-stone-100 text-6xl">6</h1>
          </div>
        </div>
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "./vue-slick-carousel-theme.css";

export default {
  name: "IndexPage",
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        dots: true,
        infinite: true,
        slidesToShow: 3,
        slidesToScroll: 1,
        autoplay: true,
        autoplaySpeed: 3000,
        pauseOnDotsHover: true,
        pauseOnFocus: true,
        pauseOnHover: true,
      },
    };
  },
};
</script>

<style scoped>
.mycontainer {
  width: 100vw;
  height: 500px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #456;
}

.mycarousel {
  height: 400px;
}

.card {
  height: 400px;
  background: #896;
}

.bg-carou {
  width: 100%;
  height: 100%;
  background: #869;
  display: flex;
  align-items: center;
  justify-content: center;
}

.content {
  width: 80%;
  height: 80%;
  background: #000;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>