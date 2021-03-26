<template>
  <ion-slides class="slides" :options="slideOpts">
    <ion-slide>
      <div class="category">
        <p>Action</p>
      </div>
    </ion-slide>
    <ion-slide>
      <div class="category">
        <p>Krime</p>
      </div>
    </ion-slide>
    <ion-slide>
      <div class="category">
        <p>Adventure</p>
      </div>
    </ion-slide>
    <ion-slide>
      <div class="category">
        <p>Erotic</p>
      </div>
    </ion-slide>
  </ion-slides>
</template>

<script>
import { IonSlides, IonSlide } from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: { IonSlides, IonSlide },
  setup() {
    // Optional parameters to pass to the swiper instance. See http://idangero.us/swiper/api/ for valid options.
    const slideOpts = {
      initialSlide: 0,
      slidesPerView: 2.8,
      spaceBetween: 0,
      centerredSlide: true,
      depth: 200,
      modifier: 1,
    };

    return { slideOpts };
  },
});
</script>
<style scoped>
ion-slide {
  padding-bottom: 20px;
}
.slides {
  margin-top: 10 px;
}
.slides img {
  border-radius: 10px;
  position: relative;
}
.slides .title {
  position: absolute;
  bottom: 0;
  color: white;
  text-align: left;
  font-weight: bold;
  padding: 10px;
  text-shadow: 1px 1px 2px grey;
}
.category {
  margin-top: 15px;
  background-color: var(--ion-color-danger);
  color: white;
  padding: 5px 25px 5px 25px;
  border-radius: 10px;
  font-size: 12px;
  font-weight: bold;
  box-shadow: -1px 11px 13px -6px var(--ion-color-danger);
}
</style>
