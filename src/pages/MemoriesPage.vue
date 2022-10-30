<template>
	<base-layout page-title="All Memories">
		<h2>These are my memories - list to be added</h2>
		<ion-list>
			<ion-item>Max</ion-item>
			<ion-item>Manuel</ion-item>
			<ion-item>Julie</ion-item>
			<ion-item>George</ion-item>
		</ion-list>
	</base-layout>
</template>

<script>
import { IonList, IonItem } from '@ionic/vue'

export default {
	components: {
		IonList,
		IonItem,
	},
}
</script>

<style scoped></style>
