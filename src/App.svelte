<script>
	import ContactList from './ContactList.svelte';
	import Experience from './Experience.svelte';
	import positions from './_positions.json';
</script>

<header>
	<h1>Kylee Tilley</h1>

	<ContactList />
</header>

<main>
	<Experience {positions} />
</main>
