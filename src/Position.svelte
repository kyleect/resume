<script>
  export let title;
  export let company;
  export let dateStart;
  export let dateEnd;
  export let location;
  export let description;
  export let items;
  export let stack;
</script>

<style>
  p {
    margin: 0;
  }

  .title {
    font-weight: bold;
    font-size: 1.1em;
  }

  .company, .description, .stack {
    margin-top: .5em;
  }

  .company, .dates, .location, .description, .stack, .skills {
    font-size: .85em;
  }

  .skills {
    padding: 0;
  }

  .stack, .skills {
    margin-top: 1em;
  }
</style>

<p class="title">{title}</p>

<p class="company">{company}</p>

<p class="dates">{dateStart} -- {dateEnd}</p>

<p class="location">{location}</p>

<p class="description">{description}</p>



{#if items}
  <ul class="skills">
    {#each items as item}
      <li>{item}</li>
    {/each}
  </ul>
{/if}

{#if stack}
  <p class="stack">Stack: {stack}</p>
{/if}