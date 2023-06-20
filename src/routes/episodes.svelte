<script>
// @ts-nocheck

  export let episodes //becomes a prop or @Input()
</script>

<nav>
  <ul>
    {#each episodes as episode}
      <li><a href={`/show/${episode?.number}`}>{episode.title}</a></li>
    {/each}
  </ul>
</nav>
