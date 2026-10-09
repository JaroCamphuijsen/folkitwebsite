

<section class="forest-section">
    <h1>Welcome to SvelteKit</h1>
    <!-- <img src={forest}> -->
    <p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
</section>

<style>
	.forest-section {
        position: relative;
        width: 100%;
        height: 1000vh;
        background-image: url('/img/forest.jpg');
        background-size: 100% auto;
        background-position: center;
        background-attachment: fixed;
        animation:  zoomOnScroll linear ;
        animation-timeline: view();
        animation-range: cover 0% cover 100%;
	}

	@keyframes zoomOnScroll {
	from {
		background-size: 100% auto;
	}
	to {
		background-size: 150% auto; /* adjusts zoom level */
	}
	}
</style>