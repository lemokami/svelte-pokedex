<script>
	import PokeCard from '../components/PokeCard.svelte';
	import { pokemon } from '../stores/pokestore';
</script>

<svelte:head>
	<title>Home Page</title>
</svelte:head>

<h1 class="text-4xl font-bold text-blue-700 text-center">Welcome to SvelteKit</h1>
<div class="grid grid-cols-1 md:grid-cols-3 gap-3 p-16">
	{#each $pokemon as pokeman (pokeman.id)}
		<PokeCard {pokeman} />
	{/each}
</div>
