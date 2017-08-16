<template lang="html">
  	<div class="">
  		<input type="text" name="" :value="msg" @input="changeMessage">
		<p>
			{{ message  }}
		</p>
  	</div>
</template>

<script>
export default {
	props : ['msg'],
	data() {
		return {
			message :''
		}
	},
	methods : {
		changeMessage (event){
			this.message = event.target.value;
			this.$emit('messageChanged', this.message);
		}
	}
}
</script>

<style lang="css">
</style>
