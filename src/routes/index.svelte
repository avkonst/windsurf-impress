<script>
	import Tailwind from '../components/Tailwind.svelte'
	import Impress from '../components/Impress.svelte'
</script>

<svelte:head>
	<title>Let's go Windsurfing</title>
</svelte:head>

<Tailwind/>
<Impress/>

<div id="impress"
    data-transition-duration="1000"
    
    data-width="1024"
    data-height="768"
    data-max-scale="3"
    data-min-scale="0"
    data-perspective="1000"
    
	data-autoplay="7">
	
	<div id="bored" class="step slide" data-x="-1000" data-y="-1500" data-autoplay="10">
        <q class="font-brand">Aren’t you just <b>bored</b> with all those slides-based presentations?</q>
    </div>
	
	<div class="step slide" data-x="0" data-y="-1500">
        <q>Don’t you think that presentations given <strong>in modern browsers</strong> shouldn’t <strong>copy the limits</strong> of ‘classic’ slide decks?</q>
    </div>

	<div class="step slide2" data-x="1000" data-y="-1500">
        <q>Slide 3</q>
    </div>
</div>
