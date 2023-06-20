<script>
  // import Test from '$lib/test.svelte';
  export let data // it is linked to +page.js through naming convention and we can get all data from the +page.js
  $: ({ latest_episode } = data)// we have destructured data same as const { latest_episode } = data; with the added feature that
  // it is reactive and will trigger change detection whenever data is renewed.
</script>
<!-- <Test/> -->
<h3>{latest_episode?.title}</h3> <!--All this data is server side rendered!!, which is amazing-->