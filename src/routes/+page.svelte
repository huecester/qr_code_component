<script lang="ts">
	import '@fontsource/outfit/400.css';
	import '@fontsource/outfit/700.css';
	import 'normalize.css/normalize.css';

	import '$lib/styles/global.scss';

	import QrCode from '$lib/components/QrCode.svelte';
</script>

<main class="center">
	<QrCode />
</main>

<style lang="scss">
	.center {
		width: 100vw;
		height: 100%;
		display: flex;
		align-items: center;
		justify-content: center;
	}
</style>
