<script>
	import { onMount } from 'svelte';
	onMount(async () => {
		await import('impress.js');
		impress().init()
	});
</script>

<style global>
    @import '../assets/impress.css';
</style>