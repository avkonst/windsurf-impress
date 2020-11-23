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
    data-perspective="0"
    
    data-media-autoplay="true"
    data-media-autostop="true"
>
    <div id="intro" class="step slide" data-x="-140" data-y="0" data-scale="10" data-rotate-x="90" _data-autoplay="10">
        <div class="w-slide h-slide flex flex-col justify-center items-center">
            <div class="w-full flex justify-center items-center">
                <div>
                    <img class="w-72 h-72" alt="" src="/sailsonic_logo_contour.svg" />
                </div>
            </div>
            <div class="p-10 font-brand uppercase text-5xl font-bold text-center">
                Let's go windsurfing!
            </div>
        </div>
    </div>    

    <div id="what" class="step slide" data-x="0" data-y="0" data-scale="1" data-rotate-x="90" data-rotate-z="90" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                What is windsurfing?
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

    <div id="why" class="step slide" data-x="0" data-y="0" data-scale="1" data-autoplay="3">
        <div class="w-slide h-slide flex flex-col justify-center items-center">
            <div class="w-full flex justify-end items-end">
                <div>
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                    <img class="w-32 h-24" alt="" src="/black-square.jpg" />
                </div>
                <div>
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                    <img class="w-32 h-16" alt="" src="/black-square.jpg" />
                </div>
                <div>
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                    <img class="w-32 h-8" alt="" src="/black-square.jpg" />
                </div>
                <div>
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                </div>
                <div>
                    <img class="w-32 h-8" alt="" src="/black-square.jpg" />
                </div>
            </div>
            <div class="p-10 font-brand uppercase text-5xl font-bold text-center">
                Why is Windsurfing good for you?
            </div>
            <div class="w-full flex justify-start items-start">
                <div>
                    <img class="w-32 h-8" alt="" src="/black-square.jpg" />
                </div>
                <div>
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                </div>
                <div>
                    <img class="w-32 h-8" alt="" src="/black-square.jpg" />
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                </div>
                <div>
                    <img class="w-32 h-16" alt="" src="/black-square.jpg" />
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                </div>
                <div>
                    <img class="w-32 h-24" alt="" src="/black-square.jpg" />
                    <img class="w-32 h-32" alt="" src="/sailsonic_logo_contour.svg" />
                </div>
            </div>
        </div>
    </div>

    <div id="it-is-fun" class="step slide" data-x="36" data-y="-196" data-scale="0.05" _data-autoplay="10">
        <div class="w-slide h-slide  flex flex-col justify-center items-center">
            <div class="p-10 w-full font-brand uppercase text-4xl font-bold text-left">
                Absolute fun. Amazing sensations. Healthy addiction.
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

    <div id="it-is-challenge" class="step slide" data-x="-12" data-y="256" data-scale="0.05" _data-autoplay="10">
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

    <div id="it-is-safe" class="step slide" data-x="164" data-y="-160" data-scale="0.05" _data-autoplay="10">
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
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-healthy" class="step slide" data-x="-144" data-y="224" data-scale="0.05" _data-autoplay="10">
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
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-environmentally-friendly" class="step slide" data-x="292" data-y="-124" data-scale="0.05" _data-autoplay="10">
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
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-affordable" class="step slide" data-x="-272" data-y="188" data-scale="0.05" _data-autoplay="10">
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

    <div id="it-is-olympic" class="step slide" data-x="420" data-y="-92" data-scale="0.05" _data-autoplay="10">
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
	<div class="step slide" data-x="0" data-y="0" data-scale="0.8" data-autoplay="0.001" />

    <div id="it-is-lifetime" class="step slide" data-x="-400" data-y="152" data-scale="0.05" _data-autoplay="10">
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

    <div id="welcome" class="step slide" data-x="-140" data-z="-5000" data-scale="6" data-rotate-x="90" data-autoplay="2">
        <div class="w-slide h-slide flex flex-col justify-center items-center">
            <div class="p-10 font-brand uppercase text-5xl font-bold text-center">
                And you can windsurf too!
            </div>
        </div>
    </div>    

    <div id="where" class="step slide" data-x="-140" data-z="10000" data-scale="6" data-rotate-x="90" _data-autoplay="10">
        <div class="w-slide h-slide flex flex-col justify-start items-center">
            <div class="p-10 font-brand uppercase text-5xl font-bold text-center">
                <span class="">Naval Point Sailing Club</span>
            </div>
            <div class="prose-2xl text-white-default">
                <h3>Where:</h3>
                <p><a href="https://www.navalpoint.co.nz/">Naval Point Sailing Club</a>, Lyttelton Harbour.</p>
                <h3>When:</h3>
                <p>Every Saturday 9:00am - 12:00am, Terms 4 and 1.<br/>
                    + all other windy days (intermediate windsurfers with own gear)
                <h3>Cost:</h3>
                <p>First year: $400 /year (gear provided)<br/>
                Subsequent years: $200 /year (your own gear required)</p>
                <h3>Contact:</h3>
                <p>+64 3 328 7029</p>
            </div>
        </div>
    </div>

</div>

<Video/>
