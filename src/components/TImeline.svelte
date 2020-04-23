<script>
  import Card from './Card.svelte'
  export let posts = []
</script>

<style>
  .Timeline {
    padding: 4em 0 0 0;
  }
</style>

<main class="Timeline">
  <div class="Timeline-container">
    	{#each posts as post}
        <Card {...post} />
      {:else}
        <p>Loading...</p>
      {/each}
  </div>
</main>
