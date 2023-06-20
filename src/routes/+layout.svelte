<script>
  import Header from './header.svelte';
  import Footer from './footer.svelte';
  import './styles.css';
	import Episodes from './episodes.svelte';
  export let data

  $: ({all_episodes} = data)
</script>

<Header/>

<main>
  <aside>
    <Episodes episodes={all_episodes}/>
  </aside>
  <div>
    <slot /> <!--Episode HTML details from paramterised route +page.svelte-->
  </div>
</main>

<Footer/>

<style>
  main {
    display: grid;
    grid-template-columns: 1fr 400px;
    gap: 20px;
  }
</style>