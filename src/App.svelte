<script>
	import ContactList from './ContactList.svelte';
	import Experience from './Experience.svelte';
	import positions from './_positions.json';
	import Position from './Position.svelte';
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

	<p>I am a software engineer with several years of experience with development, testing and how they converge when delivering a quality product. Looking for positions where I can lead feature teams towards high delivery.</p>

	<h2>Experience</h2>

	<Experience {positions} />

	<h2>Volunteer</h2>

	<Position
		title="Director of Education"
		company="Des Moines Area Quality Assurance Association"
		dateStart="Jan 2019"
		description="Working to develop the educational content and direction for the user group"
		location="Des Moines, IA Area"
	/>
</main>
