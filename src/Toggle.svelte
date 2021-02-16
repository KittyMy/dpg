<script>
	export let isActive;
	isActive = true;
	
	function toggleActive() {
//     isActive = !isActive
		
		this.classList.toggle('hide');
		
		console.log(this);
	}
</script>

<style>
	.wrapper {
		display: flex;
	}
	.one, .two, .three{
		width: 150px;
		height: 150px;
		text-align: center;
		border: 1px solid #aaa;
		margin-left: 20px;
		border-radius: 2px;
		box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
		background: red;
		opacity: 1;
	}
 	.two {
		background: blue;
	}
	.three {
		background: green;
	} 
	.hide {
		opacity: 0;
	}
	/* 	.active {
		display: none; */
/* 		opacity: 0; */
/* 	} */
</style>


<div class="wrapper">
	<div on:click|preventDefault|stopPropagation={toggleActive}>
		
		{#if isActive}
			<div class="one"></div>
		{/if}
<!-- 		{#if isActive}
			<div class="two"></div>
		{/if}
		{#if isActive}
			<div class="three"></div>
		{/if} -->
		
	</div>
</div>