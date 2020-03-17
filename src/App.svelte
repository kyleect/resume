<script>
	import ContactList from './ContactList.svelte';
	import Experience from './Experience.svelte';
	import positions from './_positions.json';
</script>

<style>
	main {
		padding: 3em;
	}

	h1 {
		margin-top: 0;
		margin-bottom: .5em;
	}
</style>

<main>
	<header>
		<h1>Kylee Tilley</h1>

		<ContactList />
	</header>

	<p>I am a software engineer with several years of experience with development, testing and how they converge to delivering a quality product. Looking for positions where I can lead feature teams towards high delivery.</p>

	<Experience {positions} />
</main>
