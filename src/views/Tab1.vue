<template>
  <ion-page>
    <ion-header class="ion-no-border primary">
      <ion-toolbar>
        <ion-title>Movies</ion-title>
        <ion-buttons slot="start">
          <ion-button>
            <ion-icon :icon="menu"></ion-icon>
          </ion-button>
        </ion-buttons>
        <ion-buttons slot="end">
          <ion-button>
            <ion-icon :icon="search"></ion-icon>
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <div class="mt-2">
        <Slides />
      </div>
      <category-slides></category-slides>
      <main-slides></main-slides>
      <main-slides></main-slides>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
  IonButtons,
  IonButton,
  IonIcon,
} from "@ionic/vue";
import Slides from "@/components/Slides.vue";
import { menu, search } from "ionicons/icons";
import CategorySlides from "@/components/CategorySlides.vue";
import MainSlides from "@/components/MainSlides.vue";

export default {
  name: "Tab1",
  components: {
    Slides,
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    IonButtons,
    IonButton,
    IonIcon,
    CategorySlides,
    MainSlides,
  },
  setup() {
    return { menu, search };
  },
};
</script>
<style scoped>
.mt-2 {
  margin-top: 2rem;
}
</style>
