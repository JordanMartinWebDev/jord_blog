<script>
	export let data;
	const { title, date, thumbnail, Content } = data;
</script>

<article>
	<img src="../{thumbnail}" alt="" />
	<h1>{title}</h1>
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
			max-width: 300px;
		}
		& h1 {
			margin-bottom: 0;
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
		}
	}
</style>
