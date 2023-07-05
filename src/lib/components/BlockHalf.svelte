<script lang="ts">
	import Intersection from '$lib/components/Intersection.svelte'
	export let image1: string
	export let image2: string
	export let title = ''
	export let invert = false
	let intersecting = false
</script>

<div class="py-24">
	<Intersection bind:intersecting class="container grid items-center gap-y-24 md:grid-cols-2">
		<div
			class="transition duration-1000"
			class:md:order-2={invert}
			class:opacity-0={!intersecting}
			class:translate-x-24={!intersecting && invert}
			class:-translate-x-24={!intersecting && !invert}
		>
			<h3 class="mb-8 font-display text-3xl">{@html title}</h3>
			<div class="prose">
				<slot />
			</div>
		</div>

		<div
			class="transition duration-1000"
			class:md:pl-8={!invert}
			class:md:pr-8={invert}
			class:xl:pl-24={!invert}
			class:xl:pr-24={invert}
			class:opacity-0={!intersecting}
			class:translate-x-24={!intersecting && !invert}
			class:-translate-x-24={!intersecting && invert}
		>
			<img class="relative z-10 w-full pl-24" src={image1} loading="lazy" decoding="async" alt="" />
			<img class="-mt-8 w-full pr-24" src={image2} loading="lazy" decoding="async" alt="" />
		</div>
	</Intersection>
</div>
