<template>
	<ion-list>
		<memory-item
			v-for="memory of memories"
			:key="memory.id"
			:memory="memory"
		></memory-item>
	</ion-list>
</template>

<script>
import { IonList } from '@ionic/vue'
import MemoryItem from './MemoryListItem.vue'

export default {
	props: ['memories'],
	components: {
		IonList,
		MemoryItem,
	},
}
</script>
