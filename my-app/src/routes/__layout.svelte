<script lang="ts">
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
import About from './about.svelte';
import Index from './index.svelte';
import Projects from './projects.svelte';
</script>

<Header />

<main>
	<Index/>
  <About/>
  <Projects/>
</main>


<style>
	main {
		margin-top: 2%;
	}

</style>
