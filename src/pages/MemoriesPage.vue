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
	data() {
		return {
			memories: [
				{
					id: 'm1',
					image:
						'https://www.exoticca.com/uk/magazine/wp-content/uploads/2021/06/matterhorn-BLOG-mountains.png',
					title: 'A trip into the mountains',
					description: 'It was a really nice trip!',
				},
				{
					id: 'm2',
					image:
						'https://media.newyorker.com/photos/5d5fd4f87ec6dc000826f2fb/16:9/w_2560,h_1440,c_limit/Brisick-Surfing-Selfie.jpg',
					title: 'Surfing the sea side',
					description: 'Feeling the cool breez',
				},
				{
					id: 'm3',
					image:
						'https://cdn.vox-cdn.com/thumbor/9qN-DmdwZE__GqwuoJIinjUXzmk=/0x0:960x646/1200x900/filters:focal(404x247:556x399)/cdn.vox-cdn.com/uploads/chorus_image/image/63084260/foodlife_2.0.jpg',
					title: 'Good eating',
					description: 'Really tasty!',
				},
			],
		}
	},
}
</script>

<style scoped></style>
