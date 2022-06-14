import { defineAsyncComponent } from 'vue';
<template>
  <div class="d-flex justify-content-center">
	<h1 class="align-self-center">No hay nada seleccionado</h1>
	
  </div>
  <FabP />
</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core'

export default {
	components: {
		FabP: defineAsyncComponent(()=> import('../components/FabP.vue'))

	}
}
</script>


<style lang="scss" scoped>
div{
	height: 100%;
}

</style>