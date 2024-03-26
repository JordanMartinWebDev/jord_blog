<footer>
	<div>
		<h4>Socials</h4>
		<ul>
			<li><a href=""><i class="fa-brands fa-github"></i></a></li>
			<li><a href=""><i class="fa-brands fa-linkedin"></i></a></li>
		</ul>
	</div>
	<div>
		<p>©2024 Jordan Martin</p>
		<p>Made with <a href="https://kit.svelte.dev/">SvelteKit</a></p>
	</div>
</footer>

<style>
	footer {
		padding: 1rem;
		background: hsl(201, 63%, 58%);
		display: grid;
		grid-template-columns: 1fr 1fr;
		justify-items: center;
		align-items: center;
		font-size: 1.5rem;
		padding: 3rem;
		color: hsl(210, 33%, 12%);
		& div:first-child {
			border-right: 1px hsl(210, 33%, 12%) solid;
			padding-right: 30%;
		}
		& a:visited {
			color: inherit;
		}
		& a:hover {
			color: hsl(49, 100%, 50%);
		}
	}
	ul {
		margin: 0;
		padding: 1rem 0;
		display: flex;
		list-style: none;
		gap: 0.5rem;
		font-size: 3rem;
	}
	h4 {
		margin: 0;
	}
	p {
		font-size: 1.4rem;
	}
</style>
