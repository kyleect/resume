<script>
	import ContactList from './ContactList.svelte';
	import Experience from './Experience.svelte';
	import positions from './_positions.json';
	import volunteer from './_volunteer.json';

	debugger;
</script>

<style>
	main {
		padding: 3em;
	}

	h1 {
		margin-top: 0;
		margin-bottom: .5em;
	}

	h2 {
		margin-top: 0;
		margin-bottom: .5em;
	}
</style>

<main>
	<header>
		<h1>Kylee Tilley</h1>

		<ContactList />
	</header>

	<p>I'm a developer with a passion for testing. Moving from hobby developer to cutting my teeth at a silicon valley startup. I've worked for several enterprise companies bringing my unique perspective to level up both developers and testers. With a passion for teaching and coaching I've spoken at several local user groups and conferences.</p>

	<h2>Experience</h2>

	<Experience {positions} />

	<h2>Volunteer</h2>

	<Experience positions={volunteer} />
</main>
