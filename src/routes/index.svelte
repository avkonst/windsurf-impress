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
    
    data-width="1200"
    data-height="900"
    data-max-scale="3"
    data-min-scale="0"
    data-perspective="1000"
    
    _data-autoplay="7"

    data-media-autoplay="true"
    data-media-autostop="true"
>
	
	<div id="why" class="step slide" data-x="0" data-y="0" data-scale="1" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="w-9/12 font-brand uppercase text-5xl font-bold text-center">
                Why is Windsurfing good for you?
            </div>
        </div>
    </div>

    <div id="it-is-fun" class="step slide" data-x="-360" data-y="-200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-end items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                Absolute fun. Amazing sensations.
            </div>
            <div>
                <video
                    _muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-fun.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="-240" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-challenge" class="step slide" data-x="-120" data-y="200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                Easy to start. Hard to advance.<br/>Never gets boring.
            </div>
            <div>
                <video
                    _muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-fun.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-safe" class="step slide" data-x="120" data-y="-200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                It is very safe.<br/>Need for an adrenaline? Go extreme.
            </div>
            <div>
                <video
                    muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-safe.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="240" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-healthy" class="step slide" data-x="360" data-y="200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                Improves physical and mental health.<br/>Full body exercise. Intense energy release.
            </div>
            <div>
                <video
                    _muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-healthy.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="360" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="slide5" class="step slide" data-x="360" data-y="-200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-center">
                It is environmentally friendly.
            </div>
            <div>
                <video
                    muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-environmentally-friendly.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="240" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-affordable" class="step slide" data-x="120" data-y="200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                It is relatively affordable sport.
            </div>
            <div>
                <video
                    _muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-fun.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-olympic" class="step slide" data-x="-120" data-y="-200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                Lots of options. And it is Olympic sport.
            </div>
            <div>
                <video
                    _muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-olympic.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="-240" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-lifetime" class="step slide" data-x="-360" data-y="200" data-scale="0.2" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                It is Lifetime sport.
            </div>
            <div>
                <video
                    _muted
                    id="my-video"
                    class="video-js"
                    _controls
                    preload="auto"
                    width="1200"
                    _height="auto"
                    poster="black-square.jpg"
                    data-setup=""
                    onended="impress().next()"
                >
                    <track kind="captions" />
                    <source src="/videos/it-is-lifetime.mp4" type="video/mp4" />
                    <!-- <source src="/videos/it-is-lifetime.webm" type="video/webm" /> -->
                    <p class="vjs-no-js">
                    To view this video please enable JavaScript, and consider upgrading to a
                    web browser that
                    <a href="https://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
                    </p>
                </video>
            </div>
        </div>
    </div>
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

</div>

<Video/>
