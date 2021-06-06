<script>
	export let pokeman;
</script>

<div class="bg-green-400 p-2 rounded-md flex flex-col items-center">
	<img src={pokeman.sprites['front_default']} alt={pokeman.name} class="h-48 bg-white rounded-md" />
	<div class="rounded-md p-2 w-full bg-white mt-2 space-y-2">
		<div class="flex justify-between w-full">
			<span class="font-semibold">Species</span>
			<span>{pokeman.species.name}</span>
		</div>
		<div class="flex justify-between w-full">
			<span class="font-semibold">Height</span>
			<span>{pokeman.height}</span>
		</div>
		<div class="flex justify-between w-full">
			<span class="font-semibold">Weight</span>
			<span>{pokeman.weight}</span>
		</div>
		<div class="flex justify-between w-full">
			<span class="font-semibold">Type</span>
			<span>{pokeman.types[0].type.name}</span>
		</div>
	</div>
</div>
