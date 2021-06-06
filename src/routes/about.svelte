<svelte:head>
	<title>About Page</title>
</svelte:head>

<div class="flex items-center flex-col justify-center space-y-4 px-16 text-center">
	<h2 class="text-4xl text-green-900 font-bold">Pokedex using SvelteKit</h2>
	<p class="text-center text-xl max-w-xl">
		This is a result from my effort to learn <a
			class="svelte-color"
			href="https://kit.svelte.dev/"
			target="_blank">sveltekit</a
		>. I learned a lot from this project and it made love
		<a class="svelte-color" href="https://svelte.dev" target="_blank">svelte</a>
		even more. This project is on
		<a href="https://github.com/lemokami/svelte-pokedex" target="_blank">github</a>
	</p>
</div>

<style>
	a {
		@apply underline font-bold;
	}
	.svelte-color {
		@apply text-red-400;
	}
</style>
