<template>
  <ion-slides class="slides" :options="slideOpts">
    <ion-slide>
      <div>
        <p>Action</p>
      </div>
    </ion-slide>
    <ion-slide>
      <div>
        <p>Krime</p>
      </div>
    </ion-slide>
    <ion-slide>
      <div>
        <p>Adventure</p>
      </div>
    </ion-slide>
    <ion-slide>
      <div>
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
      slidesPerView: 1.2,
      spaceBetween: 50,
      centerredSlide: true,
      speed: 400,
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
</style>
