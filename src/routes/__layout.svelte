<script>
	import Nav from './../components/nav.svelte';
	import Contact from './../components/contact.svelte';
</script>

<Nav />
<slot />
<Contact />

<style>
	@import './../global.css';
</style>
