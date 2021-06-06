<script>
	import Navbar from '../components/Navbar.svelte';
</script>

<Navbar />
<div class="flex flex-col items-center px-16">
	<slot />
</div>

<style>
	@tailwind base;
	@tailwind components;
	@tailwind utilities;
</style>
