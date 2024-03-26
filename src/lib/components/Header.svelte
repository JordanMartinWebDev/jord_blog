<script>
	import logo from '$lib/assets/Full Logo.svg';
</script>

<header>
	<a href="/"
		><img alt="The project logo" src={logo} />
		<h3>Jordan Martin</h3></a
	>

	<nav>
		<ul>
			<li>
				<a href="/blog">Blog</a>
			</li>
			<li>
				<a href="/projects">Projects</a>
			</li>
			<li>
				<a href="/about">About</a>
			</li>
			<li>
				<a href="/contact">Contact</a>
			</li>
		</ul>
	</nav>
</header>

<style>
	header {
		font-size: 2rem;
		margin: 2rem auto 0 auto;
		padding: 1rem 0 3rem 0;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		align-items: center;
		max-width: 90%;
		border-bottom: 1px hsl(201, 63%, 58%) solid;
	}

	ul {
		margin: 0;
		list-style-type: none;
		display: flex;
		gap: 1rem;
	}

	a {
		text-decoration: none;
		color: inherit;
		display: flex;
		gap: 15px;
		& h3 {
			font-weight: 400;
			margin: 0;
		}
	}

	img {
		width: 3.6rem;
	}
</style>
