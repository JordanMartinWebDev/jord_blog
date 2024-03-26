<script>
	export let data;
</script>

<section>
	<h3>current = getBlogPosts()</h3>
	<h2>Blog</h2>

	<ul>
		{#each data.posts as post}
			<li>
				<card>
					<img src={post.meta.thumbnail} alt="" />
					<div>
						<h2>
							<a href={post.path}>
								{post.meta.title}
							</a>
						</h2>
						<p>{post.meta.description}</p>
						<p class="published">Published {post.meta.date}</p>
					</div>
				</card>
			</li>
		{/each}
	</ul>
</section>

<style>
	section {
		& a {
			color: inherit;
		}
		& ul {
			display: grid;
			grid-template-columns: 1fr 1fr;
			list-style: none;
			padding: 0 1rem;
			color: hsl(0, 0, 99%);
			& card {
				display: flex;
				gap: 20px;
			}
			& img {
				max-width: 300px;
			}
			& li {
				padding: 1rem 1rem;
				margin-right: 5rem;
				margin-bottom: 4rem;
				& p {
					margin: 1rem 0;
				}
				& .published {
					border-top: 1px white solid;
					padding-top: 0.5rem;
					opacity: 80%;
					font-size: 1rem;
				}
				& h2 {
					margin: 1rem 0;
				}
			}
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
</style>
