<script lang="ts">
  import Nav from '$lib/components/Nav.svelte';
  import Hero from '$lib/components/sections/Hero.svelte';
  import About from '$lib/components/sections/About.svelte';
  import Experience from '$lib/components/sections/Experience.svelte';
  import Education from '$lib/components/sections/Education.svelte';
  import Skills from '$lib/components/sections/Skills.svelte';
  import Achievements from '$lib/components/sections/Achievements.svelte';
  import Contact from '$lib/components/sections/Contact.svelte';
</script>

<Nav />
<main>
  <Hero />
  <About />
  <Experience />
  <Education />
  <Skills />
  <Achievements />
  <Contact />
</main>
