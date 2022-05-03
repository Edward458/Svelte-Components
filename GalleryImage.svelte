<script>
// Image will also be a link to view the image in a separate view
	export let link;
	export let src;
	export let alt
</script>

<a href={link}> 
	
	
<img src={src} alt={alt}>

	
</a>

<style>

	img{
		transition: transform 500ms ease;
		width: 200px;
    height: 200px;
	margin-right: 5px;
	}
	
	img:hover{
transform:scale(1.05);
	}
	
</style>