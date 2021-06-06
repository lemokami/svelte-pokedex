<script>
	export let pokeman;
</script>

<a
	href={`/pokemon/${pokeman.id}`}
	class="rounded-md bg-green-50 flex flex-col items-center justify-center cursor-pointer transition hover:shadow-lg py-5"
>
	<img src={pokeman.image} alt={pokeman.name} class="h-48" />
	<p class="uppercase tracking-wide font-medium text-green-900">{pokeman.name}</p>
</a>
