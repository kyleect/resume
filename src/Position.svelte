<script>
  export let title;
  export let company;
  export let dateStart;
  export let dateEnd;
  export let location;
  export let description;
  export let items;
</script>

<style>
  p {
    margin: 0;
  }

  .title {
    font-weight: bold;
  }
</style>

<p class="title">{title}</p>

<p class="company">{company}</p>

<p class="dates">{dateStart}-{dateEnd}</p>

<p class="location">{location}</p>

<p>{description}</p>

{#if items}
  <ul>
    {#each items as item}
      <li>{item}</li>
    {/each}
  </ul>
{/if}