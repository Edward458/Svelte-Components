<script>
// List with a button instead of a link
	// The button logic will be handled inside the component
	// The dropdown items will be SidebarItem components 
	
	let open = false;
</script>

<li>
<button on:click={() => {
	open = !open;
	}}>
	<slot name="text"/>
	</button>
	{#if open}
	<slot name="drop-list" />
	{/if}
</li>

<style>
	
	button{
		border-style:none;
		background-color:white;
		margin:0;
		padding:0;
color:rgba(40, 40, 40, 0.5);
		cursor:pointer;
	}
	
	button:active{
		background-color:white;
	}
	
	button:hover{
		color:black;
	}
</style>