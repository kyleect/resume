<script>
  import Position from './Position.svelte';

  export let positions = [];
</script>

<h2>Experience</h2>

{#each positions as position}
  <Position
    title={position.title}
    company={position.company}
    dateStart={position.dateStart}
    dateEnd={position.dateEnd}
    location={position.location}
    description={position.description}
    items={position.items}
  />
{/each}