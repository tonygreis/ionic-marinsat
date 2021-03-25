<template>
  <ion-card>
    <img
      src="https://www.themoviedb.org/t/p/w220_and_h330_face/zeD4PabP6099gpE0STWJrJrCBCs.jpg"
    />
    <ion-card-header>
      <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
      <ion-card-title>Card Title</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Keep close to Nature's heart... and break clear away, once in awhile, and
      climb a mountain or spend a week in the woods. Wash your spirit clean.
    </ion-card-content>
  </ion-card>
</template>

<script>
import {
  IonCard,
  IonCardContent,
  IonCardSubtitle,
  IonCardTitle,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: {
    IonCard,
    IonCardContent,
    IonCardSubtitle,
    IonCardTitle,
  },
  setup() {
    return {};
  },
});
</script>
<style scoped>
.card-background-page ion-card {
  position: relative;
  text-align: center;
}
.card-background-page .card-title {
  position: absolute;
  top: 36%;
  font-size: 2em;
  width: 100%;
  font-weight: bold;
  color: #fff;
}
.card-background-page .card-subtitle {
  font-size: 1em;
  position: absolute;
  top: 52%;
  width: 100%;
  color: #fff;
}
</style>
