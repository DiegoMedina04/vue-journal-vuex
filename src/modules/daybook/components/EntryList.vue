<template>
	<div class="entry-list-container">
		<div class="px-2 pt-2">
			<input type="text" class="form-control" placeholder="Buscar entrada">
		</div>
		<div class="entry-scrollarea">
			<EntryP
			v-for="i in 10" :key="i" 
			/>

		</div>
	</div>
</template>
<script>
import { defineAsyncComponent } from '@vue/runtime-core'

export default {
	components:{
		EntryP: defineAsyncComponent(()=>import('./EntryP.vue'))
	}
	
}
</script>
<style lang="scss" scoped>
.entry-list-container{
	border-right: 1px solid #2c3e50;
	height: calc(100vh - 56px);
}
.entry-scrollarea{
	height: calc(100vh - 120px);
	overflow: scroll;
}

</style>