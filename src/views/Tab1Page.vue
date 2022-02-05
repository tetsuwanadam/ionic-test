<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>
    
			<ion-list>
				<ion-item>
					<ion-label position="stacked">Test</ion-label>

					<ion-input v-model="test"></ion-input>
				</ion-item>
			</ion-list>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonList, IonItem, IonLabel, IonInput } from '@ionic/vue';

export default  defineComponent({
  name: 'Tab1Page',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonList, IonItem, IonLabel, IonInput },
  setup: function() {
    const test = ref('Test input default value');
    return {
      test,
    };
  }
});
</script>
