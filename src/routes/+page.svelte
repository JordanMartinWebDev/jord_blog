<script>
	import bracketOpen from '$lib/assets/Logo Open.svg';
	import bracketClose from '$lib/assets/Logo Close.svg';
</script>

<container>
	<section class="section1">
		<h3>current = intro();</h3>
		<div>
			<h1><strong>Hello, I'm Jordan</strong>. Full Stack Developer & Lifetime Learner.</h1>
			<h2>I live in Livingston, Louisiana, and work for NGA.</h2>
			<h4>
				This is a place for me to show my projects and what I learn from them. Call it a portfolio,
				call it a blog. Either way, it's a place where I can show what I've been up to.
			</h4>
			<ul>
				<li>
					<a href="./blog"
						><i class="fa-solid fa-file-invoice"></i>Check out what I've been learning</a
					>
				</li>
				<li>
					<a href="./projects"><i class="fa-solid fa-diagram-project"></i>Some of my projects</a>
				</li>
				<li><a href="./about"><i class="fa-solid fa-person"></i>More about me</a></li>
				<li><a href="./contact"><i class="fa-solid fa-envelope"></i>Get in touch</a></li>
			</ul>
		</div>
	</section>
</container>

<style>
	.section1 {
		& div {
			max-width: 50%;
		}
	}
	h3 {
		font-size: 2rem;
		font-weight: 300;
		background: linear-gradient(to right, hsl(201, 63%, 58%) 0%, hsl(49, 100%, 50%) 20%);
		background-clip: initial;
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}
	h4 {
		font-size: 2rem;
		font-weight: 300;
	}
	ul {
		margin: 0;
		padding: 0;
		list-style: none;
		& li {
			font-size: 2rem;
			margin: 2rem 0;
			& i {
				color: hsl(49, 100%, 50%);
				width: 35px;
				padding-right: 10px;
			}
			& a:visited {
				color: inherit;
			}
		}
	}
</style>
