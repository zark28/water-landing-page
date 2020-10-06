<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		
		width: 80vw;
		height: 80vh;
		margin: 0 auto;
		border: .5em solid #000;
		border-radius: .3em;
	}

	/* span{
		background-color: rgba(0, 0, 0, 0.651);
		display: block;
		height: 10vh;
		width: 80vw;
	} */
</style>



<main class='layout'>
		<Nav {segment}/>
	<slot></slot>
</main>