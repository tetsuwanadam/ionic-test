<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Time Picker Test</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Time Picker Test</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-item detail="true">
        <ion-label id="time_label">Show time picker</ion-label>
      </ion-item>

      <ion-popover trigger="time_label">
        <ion-datetime value="13:15" presentation="time" show-default-buttons></ion-datetime>
      </ion-popover>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonDatetime, IonHeader, IonItem, IonLabel, IonPage, IonPopover, IonTitle, IonToolbar } from '@ionic/vue';
</script>

<style scoped>
#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
