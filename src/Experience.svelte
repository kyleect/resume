<script>
  import Position from './Position.svelte';

  export let positions = [];
</script>

<style>
  ul {
    list-style: none;
    padding-left: 0;
  }

  li {
    margin-bottom: 1em;
    page-break-inside: avoid;
  }
</style>

{#if positions}
  <ul>
  {#each positions as position}
    <li>
      <Position
        title={position.title}
        subposition={position.subposition}
        company={position.company}
        dateStart={position.dateStart}
        dateEnd={position.dateEnd}
        location={position.location}
        description={position.description}
        stack={position.stack}
        items={position.items}
      />
    </li>
  {/each}
  </ul>
{/if}