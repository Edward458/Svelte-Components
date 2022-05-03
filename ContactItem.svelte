<script>
	export let link;
</script>

<p>
	<slot name="contact-title"/>
	<a href={link}>
	<slot name="contact-username"/>
	</a>
</p>

<style>
	a{
		color:black;
		text-decoration:none;
	}
	
	a:hover{
		text-decoration:none;
	}
	
	p{
		color:black;
		margin:0;
		
	}
</style>