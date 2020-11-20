<script>
	import { onMount } from 'svelte';

	onMount(async () => {
		const impressjs = await import('impress.js');
		
		impress().init()
	});
</script>

<style>
	h1, figure, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>

<svelte:head>
	<title>Let's go Windsurfing</title>
</svelte:head>

<div id="impress"
    data-transition-duration="1000"
    
    data-width="1024"
    data-height="768"
    data-max-scale="3"
    data-min-scale="0"
    data-perspective="1000"
    
	data-autoplay="7">
	
	<div id="bored" class="step slide" data-x="-1000" data-y="-1500" data-autoplay="10">
        <q>Aren’t you just <b>bored</b> with all those slides-based presentations?</q>
    </div>
	
	<div class="step slide" data-x="0" data-y="-1500">
        <q>Don’t you think that presentations given <strong>in modern browsers</strong> shouldn’t <strong>copy the limits</strong> of ‘classic’ slide decks?</q>
    </div>
</div>
