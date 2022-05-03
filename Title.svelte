<script>
// Simple title
	// Similiar to the SidebarItem, but with an h2 tag and a link instead of a li tag and a link
export let link;
</script>

<h2>
	<a href={link}>
	<slot/>
	</a>
</h2>


<style>
	a{
		color:black;
		text-decoration:none;
	}
</style>