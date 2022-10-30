<template>
	<ion-page>
		<ion-header>
			<ion-toolbar>
				<ion-title>All Memories</ion-title>
			</ion-toolbar>
		</ion-header>
		<ion-content>
			<h2>These are my memories - list to be added</h2>
			<ion-list>
				<ion-item>Max</ion-item>
				<ion-item>Manuel</ion-item>
				<ion-item>Julie</ion-item>
				<ion-item>George</ion-item>
			</ion-list>
		</ion-content>
	</ion-page>
</template>

<script>
import {
	IonPage,
	IonHeader,
	IonToolbar,
	IonTitle,
	IonContent,
	IonList,
	IonItem,
} from '@ionic/vue'

export default {
	components: {
		IonPage,
		IonHeader,
		IonToolbar,
		IonTitle,
		IonContent,
		IonList,
		IonItem,
	},
}
</script>

<style scoped></style>
