<script lang="ts">
  import { onMount } from 'svelte';
  import { skillCategories } from '$lib/data/skills.js';

  let sectionEl: HTMLElement;

  onMount(() => {
    const observer = new IntersectionObserver(
      ([entry]) => {
        if (entry.isIntersecting) {
          sectionEl.classList.add('section-visible');
          observer.disconnect();
        }
      },
      { threshold: 0.1 }
    );
    observer.observe(sectionEl);
    return () => observer.disconnect();
  });
</script>

<section id="skills" bind:this={sectionEl} class="section-animate" style="background:white;padding:80px 24px;">
  <div style="max-width:1000px;margin:0 auto;">
    <p style="font-family:var(--font-inter);font-size:0.75rem;font-weight:600;letter-spacing:0.1em;color:var(--gold);text-transform:uppercase;margin-bottom:12px;">SKILLS</p>
    <h2 style="font-family:var(--font-playfair);font-size:clamp(1.75rem,4vw,2.5rem);color:var(--navy);margin-bottom:40px;">Capabilities &amp; Credentials</h2>
    <div style="display:flex;flex-direction:column;gap:36px;">
      {#each skillCategories as category}
        <div>
          <h3 style="font-family:var(--font-inter);font-size:0.875rem;font-weight:600;color:var(--muted);text-transform:uppercase;letter-spacing:0.06em;margin-bottom:14px;">{category.label}</h3>
          <div style="display:flex;flex-wrap:wrap;gap:10px;">
            {#each category.skills as skill}
              <span style="font-family:var(--font-inter);font-size:0.875rem;font-weight:500;color:var(--navy);background:var(--highlight);border:1px solid #d0dbf0;padding:6px 14px;border-radius:99px;display:inline-flex;align-items:center;gap:6px;">
                {skill.name}
                {#if skill.certified}
                  <span style="color:var(--gold);font-size:0.75rem;" title="LinkedIn Assessment Certified">★</span>
                {/if}
              </span>
            {/each}
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
