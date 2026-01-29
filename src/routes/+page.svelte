<script>
	let components = [
		{ c: 4, r: 3 },
		{ c: 8, r: 1 },
		{ c: 8, r: 2 },
		{ c: 8, r: 1 },
		{ c: 4, r: 1 }
	];
</script>

<div class="grid grid-cols-12 grid-flow-row gap-4">
	{#each components as { c, r }}
		<div class="col-span-{c} row-span-{r} min-h-{r}0 bg-fuchsia-950"></div>
	{/each}
	<div class="col-span-4 row-span-3 min-h-30 rounded-4xl bg-amber-600"></div>
	<div class="col-span-8 rounded-4xl min-h-10 bg-amber-500"></div>
	<div class="col-span-8 row-span-2 min-h-20 rounded-4xl bg-amber-400"></div>
	<div class="col-span-8 rounded-4xl min-h-10 bg-fuchsia-500"></div>
	<div class="col-span-4 rounded-4xl min-h-10 bg-blue-600"></div>
</div>
