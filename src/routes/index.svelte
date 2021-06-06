<script>
	import PokeCard from '../components/PokeCard.svelte';
	import { pokemon } from '../stores/pokestore';

	let searchInput = '';
	let filteredPokemon = [];

	$: {
		if (searchInput) {
			filteredPokemon = $pokemon.filter((pokeman) =>
				pokeman.name.toLowerCase().includes(searchInput.toLowerCase())
			);
		} else {
			filteredPokemon = [...$pokemon];
		}
	}
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<h1 class="text-4xl font-bold text-green-800 uppercase tracking-wide text-center pb-8">
	SvelteKit pokedex
</h1>
<input
	type="text"
	bind:value={searchInput}
	class="ring-1 border-green-400 rounded-md p-2 w-full focus:outline-none focus:ring-2 ring-green-400 focus:ring-offset-2"
	placeholder="Search for your favourite pokemon"
/>
<div class="grid grid-cols-1 md:grid-cols-3 gap-3 py-4 w-full">
	{#each filteredPokemon as pokeman (pokeman.id)}
		<PokeCard {pokeman} />
	{/each}
</div>
