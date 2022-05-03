<script>
// A slighlty modified list version
	// Is a list item with a link
	export let link;
</script>

<li>
<a href={link}>
	<slot/>
	</a>
</li>

<style>
	a:hover{
		text-decoration:none;
		color:black;
	}
	
	a{
		color:rgba(40, 40, 40, 0.5);
		text-decoration: none;
	}
</style>