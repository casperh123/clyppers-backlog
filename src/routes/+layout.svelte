<script lang="ts">
	import '../app.css';
	import { Footer, Header } from '$lib/components/layout';
	let { children } = $props();
</script>

<Header />

<div class="main-wrapper">
	<div class="main-section">
		{@render children()}
	</div>
</div>

<Footer />

<style>
	.main-wrapper {
		display: flex;
		justify-content: center;
		width: 100%;
	}

	.main-section {
		width: 100%;
		max-width: 1080px;
		padding: 40px 20px;
	}
</style>
