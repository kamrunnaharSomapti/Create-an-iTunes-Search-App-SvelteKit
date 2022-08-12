<script>
	import '../app.css';
	import Header from '../components/Header.svelte';
</script>

<Header />
<div class="w-full min-h-screen bg-slate-800 px-10 md:px-20 lg:px-52 py-5">
	<slot />
</div>
