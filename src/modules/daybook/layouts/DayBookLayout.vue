<template>
    <NavbarP />
	<div class="d-flex">
		<div class="col-4">
			<EntryList/>
		</div>
		<div class="col">
			<router-view />
		</div>
	</div>
   
</template>



<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        NavbarP: defineAsyncComponent(() => import('../components/NavbarP.vue')),
		EntryList:defineAsyncComponent(() => import('../components/EntryList.vue')),
       
    }
}
</script>