<template>
  <ion-item lines="none">
    My List
    <ion-buttons slot="end">
      <ion-button>
        <ion-icon :icon="chevronForward"></ion-icon>
      </ion-button>
    </ion-buttons>
  </ion-item>
  <ion-slides class="listSlides" :options="slideOpts">
    <ion-slide>
      <div>
        <img
          src="https://www.themoviedb.org/t/p/w220_and_h330_face/zeD4PabP6099gpE0STWJrJrCBCs.jpg"
        />
      </div>
    </ion-slide>
    <ion-slide>
      <div>
        <img
          src="https://www.themoviedb.org/t/p/w220_and_h330_face/zeD4PabP6099gpE0STWJrJrCBCs.jpg"
        />
      </div>
    </ion-slide>
    <ion-slide>
      <div>
        <img
          src="https://www.themoviedb.org/t/p/w220_and_h330_face/zeD4PabP6099gpE0STWJrJrCBCs.jpg"
        />
      </div>
    </ion-slide>
  </ion-slides>
</template>

<script>
import { chevronForward } from "ionicons/icons";
export default {
  setup() {
    // Optional parameters to pass to the swiper instance. See http://idangero.us/swiper/api/ for valid options.
    const slideOpts = {
      initialSlide: 0,
      slidesPerView: 2.4,
      spaceBetween: 20,
      centerredSlide: true,
      depth: 200,
      modifier: 1,
    };

    return { slideOpts, chevronForward };
  },
};
</script>

<style scoped>
.listSlides {
}
.listSlides img {
  border-radius: 10px;
  min-height: 200px;
  max-height: 200px;
  box-shadow: -1px 11px 13px -6px rgb(87, 86, 86);
}
</style>
