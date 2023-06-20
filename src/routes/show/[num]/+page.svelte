<script>
  export let data

  $: ({ episode } = data)
</script>
<a href="/">Home</a>
<h1>{episode.title}</h1>
{@html episode.html}