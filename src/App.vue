<template>
  <ion-menu content-id="main-content">
    <!-- <ion-header>
      <ion-toolbar>
        <ion-title>Menu Content</ion-title>
      </ion-toolbar>
    </ion-header>
    
    <ion-content class="ion-padding">This is the menu content.</ion-content>
    -->
    
  </ion-menu>
  <ion-page id="main-content">
    <ion-header>
      <ion-toolbar text-align="right">
        <!-- <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons> -->

        <ion-title style="background:black;">
          <div id="titles"> 
            <ul class="nav">
              <li style="float:right"><a class="active" href="#about">Shop</a></li>
              <li ><a>About Us</a></li> 
              <li ><a>Safety</a></li>
              <li ><a>Home</a></li>
              <li style="float:left"><h1 class="name-title" href="">Trekk</h1></li>
            </ul>
          </div>
        </ion-title>
        <div id="logoWrapper" class="wrapper" data-content-field="site-title">
            
          <h1 id="logoImage"><a href="/"><img src="@/assets/Trekk-Logo.png" alt="TREKKSCOOTER"></a></h1>
          
        </div>
      </ion-toolbar>
      
    </ion-header>
    <ion-content class="ion-padding">
      Tap the button in the toolbar to open the menu.
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  //IonButtons,
  IonContent,
  IonHeader,
  IonMenu,
  //IonMenuButton,
  IonPage,
  IonTitle,
  IonToolbar,
} from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
    //IonButtons,
    IonContent,
    IonHeader,
    IonMenu,
    //IonMenuButton,
    IonPage,
    IonTitle,
    IonToolbar,
  },
});
</script>

<style scoped>
 /* #titles{
   width: 100%;
   height: 25px;
   background: rgb(7, 7, 7);
  }*/
  ul {
  list-style-type: none;
  margin: 0;
  padding: 5px;
  overflow: hidden;
  background-color: black;
}


li a {
  float: right;
  display: block;
  color: white;
  text-align: center;
  padding:16px ;
  text-decoration: none;
}

li a:hover:not(.active) {
  background-color: #111;
}

.active {
  color:black;
  background-color: yellow;
  border-radius: 300px;
  float: right;
}
.name-title {
  color:white;
  float: left;
}
#logoImage img {
    height: auto;
    max-height: 100px;
    width: auto;
    max-width: 100%;
}
img {
    border: 0;
}

:before, :after {
    box-sizing: inherit;
}
img {
    overflow-clip-margin: content-box;
    overflow: clip;
}
</style>
