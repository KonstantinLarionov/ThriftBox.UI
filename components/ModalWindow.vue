<template>
	<div class="modal">
		<div class="modal_header">	
			{{modal_header_title}}		
		</div> 
		<div class="modal_content">
			<slot>Placeholder</slot>
		</div>
		<div class="modal_footer">
			
		</div>
	</div>
</template>
<script>
export default{
	name:"ModalWindow",
	props: {
		modal_header_title:{
			type: String,
			default:"Название окна",
		}
	},
	data(){
		return{}
	},
	computed:{}
}
</script>
<style>
@import "../assets/modalwindow.scss";
</style>