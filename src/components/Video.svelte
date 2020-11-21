<script lang="js">
    import { onMount } from 'svelte';
	onMount(async () => {
		await import('video.js');
	});
</script>

<style global>
    @import 'video.js/dist/video-js.css';
</style>