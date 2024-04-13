<script>
	export let data;
	const { title, date, thumbnail, Content } = data;
</script>

<article>
	<img src="../{thumbnail}" alt="" />
	<p>Published: {date}</p>
	<Content />
</article>

<style>
	article {
		display: flex;
		align-items: left;
		flex-direction: column;
		margin: 0 25%;
		& img {
			max-width: 200px;
		}
		& h1 {
			margin-top: 0rem;
			margin-bottom: 6rem;
		}
		& h2 {
			font-size: 3rem;
		}
		& h3 {
			font-size: 2rem;
		}
		& p {
			font-size: 1.8rem;
			margin: 1rem 0;
			line-height: 2.5rem;
		}
		& ul {
			font-size: 1.8rem;
		}
		& li {
			margin-bottom: 2rem;
		}
	}
</style>
