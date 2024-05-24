<script>
	import '../app.css';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';

	let y;
	let innerHeight = 0;
	let innerWidth = 0;

	function goTop() {
		//window.scrollTo({ top: 0, behavior: 'smooth' });
		document.body.scrollIntoView();
	}
</script>

<div class="relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen">
	<div
		class={'fixed bottom-0 w-full duration-200 p-10 z-[10]' + y > 0
			? 'opacity-full pointer-events-auto'
			: 'pointer-events-none opacity-0'}
	>
		<button><i class="fa-solid fa-arrow-up"></i></button>
	</div>
	<Header {y} />
	<slot />
	<Footer />
</div>

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
