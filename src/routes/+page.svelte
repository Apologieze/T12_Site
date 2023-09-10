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
			<Card name="Momozhok" src="/img/momozhok.jpg" desc="OH LE FLOP"></Card>
			<Card name="Wataa" src="/img/wata.jpg" desc="A gagné 10€ de cash prize à un tournoi clash royal"></Card>
			<Card name="Cassoule" src="/img/milo.jpg" desc="Est allé au stade 2 de la qualification des worlds de Call of Duty mobile"></Card>
			<Card name="Azu" src="/img/sami.jpg" desc="Change 5 fois de photo de profile Discord par jour"></Card>
		</div>
	</div>
</div>
