<script>
	export let pokeman;
</script>

<a
	href={`/pokeman/${pokeman.id}`}
	class="rounded-md bg-blue-200 flex flex-col items-center justify-center cursor-pointer transition hover:shadow-lg"
>
	<img src={pokeman.image} alt={pokeman.name} class="h-48" />
	<p>{pokeman.name}</p>
</a>
