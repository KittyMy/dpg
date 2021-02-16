<script>
	import Box from './Box.svelte';
	import Toggle from './Toggle.svelte';

</script>

<Box></Box>

<style>
/* 	.active {
		display: none;
	} */
	
/* 	.one, .two, .three{
		width: 150px;
		height: 150px;
		text-align: center;
		border: 1px solid #aaa;
		margin-left: 20px;
		border-radius: 2px;
		box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
		background: red;
		opacity: 1;
	} */
	
</style>

<Toggle>
	  <div class="content" >
		The Content
	 </div>
	 <div class="content">
		The Content
	 </div>
	 <div class="content">
		The Content
	 </div>
</Toggle>