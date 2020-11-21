<script>
	import Tailwind from '../components/Tailwind.svelte'
    import Impress from '../components/Impress.svelte'
    import Video from '../components/Video.svelte'
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
        <p class="font-brand">Aren’t you just <b>bored</b> with all those slides-based presentations?</p>
    </div>
	
	<div class="step slide" data-x="0" data-y="-1500">
        <q>Don’t you think that presentations given <strong>in modern browsers</strong> shouldn’t <strong>copy the limits</strong> of ‘classic’ slide decks?</q>
    </div>

	<div class="step slide" data-x="1000" data-y="-1500">
        <q class="font-brand">Slide 3</q>
        <video
            muted
            id="my-video"
            class="video-js"
            controls
            preload="auto"
            width="640"
            height="264"
            poster="MY_VIDEO_POSTER.jpg"
            data-setup=""
        >
            <track kind="captions" />
            <source src="/videos/it-is-lifetime.mp4" type="video/mp4" />
            <!-- <source src="MY_VIDEO.webm" type="video/webm" /> -->
            <p class="vjs-no-js">
            To view this video please enable JavaScript, and consider upgrading to a
            web browser that
            <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
            </p>
        </video>
    </div>
</div>

<Video/>
