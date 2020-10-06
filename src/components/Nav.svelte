<script>
	export let segment;
</script>

<style>
	nav {

		/* border-bottom: 1px solid rgba(255,62,0,0.1); */
		font-weight: 300;
		padding: 1em 5em;
		background: rgba(0, 0, 0, 0.151);
		display: flex;
		justify-content: space-between;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
		margin:0 2em ;
		font-weight: 200;
		font-size: 2em;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(119, 109, 106);
		display: block;
		top: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}

	.logo{
		width: 3em;
	}
	.search{
		width: 2em;
		font-weight: 400 ;
	}
</style>

<nav>
	<img class='logo' src="vibrate.svg" alt="">
	<ul>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">Home</a></li>
		<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">About Us</a></li>
		<li><a aria-current="{segment === 'shop' ? 'page' : undefined}" href="shop">Shop</a></li>
		<li><a aria-current="{segment === 'contactus' ? 'page' : undefined}" href="contactus">Contact Us</a></li>
	</ul>
	<img class='search' src="search.svg" alt="">
</nav>
