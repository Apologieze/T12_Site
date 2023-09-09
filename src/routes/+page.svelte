<script>
	import Card from "../card.svelte";
	import { AppBar } from '@skeletonlabs/skeleton';
</script>

<div class="page h-screen">
	<AppBar class="flex items-center justify-center" gap="gap-0" background="bg-surface-900/40">
		<div class="box-header flex justify-center w-full">
			<h1 class="h1">T12 ESPORT</h1>
		</div>
	</AppBar>

	<div class="box container mx-auto flex items-center flex-col h-full gap-8 p-4">
		<h2 class="h2">Feur</h2>
		<div class="carte flex justify-center gap-10">
			<Card name="Momozhok" src="/img/momozhok.jpg"></Card>
			<Card name="Wataa" src="/img/wata.jpg"></Card>
		</div>
	</div>
</div>
