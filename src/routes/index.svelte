<script>
	import { goto } from '$app/navigation';
	let searched = '';
	const search = () => {
		goto(`${searched}`);
	};
</script>

<section>
	<div class="flex flex-col items-center justify-center h-screen">
		<div class="text-white text-5xl capitalize pb-10">search an artist</div>
		<div
			class="w-full md:w-96 flex justify-between rounded-md bg-white bg-opacity-20 p-1 border border-white border-opacity-30"
		>
			<input
				class="w-4/5 p-2 bg-transparent border border-slate-600 rounded-xl focus:outline-0"
				type="text"
				bind:value={searched}
			/>
			<button on:click={search} class=" w-1/4 p-2 ml-4 rounded-md bg-white font-medium "
				>search</button
			>
		</div>
	</div>
</section>
