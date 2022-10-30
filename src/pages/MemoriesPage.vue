<template>
	<base-layout page-title="All Memories">
		<ion-list>
			<ion-item
				v-for="memory of memories"
				:key="memory.id"
				:router-link="`/memories/${memory.id}`"
			>
				<ion-thumbnail slot="start">
					<ion-img :src="memory.image"></ion-img>
				</ion-thumbnail>
				<ion-label>
					{{ memory.title }}
				</ion-label>
			</ion-item>
		</ion-list>
	</base-layout>
</template>

<script>
import { IonList, IonItem, IonImg, IonThumbnail, IonLabel } from '@ionic/vue'

export default {
	components: {
		IonList,
		IonItem,
		IonImg,
		IonThumbnail,
		IonLabel,
	},
	computed: {
		memories() {
			return this.$store.getters.memories
		},
	},
}
</script>

<style scoped></style>
