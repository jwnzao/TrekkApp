<template>
  <ion-menu content-id="main-content">
    <ion-header>
      <ion-toolbar>
        <ion-title>Menu Content</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">This is the menu content.</ion-content>
  </ion-menu>
  <ion-page id="main-content" text-align="left">
    <ion-header>
      <ion-toolbar text-align="right">
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>

        <ion-title style="background:black;">
          <div id="titles"> 
            <ul class="nav">
            </ul>
          </div>
        </ion-title>
      </ion-toolbar>
      
    </ion-header>
    <ion-content class="ion-padding">
      Tap the button in the toolbar to open the menu.
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonButtons,
  IonContent,
  IonHeader,
  IonMenu,
  IonMenuButton,
  IonPage,
  IonTitle,
  IonToolbar,
} from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
    IonButtons,
    IonContent,
    IonHeader,
    IonMenu,
    IonMenuButton,
    IonPage,
    IonTitle,
    IonToolbar,
  },
});
</script>