<script lang="ts">
  import { onMount } from 'svelte';
  import { base } from '$app/paths';
  import { education } from '$lib/data/education.js';

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

<section id="education" bind:this={sectionEl} class="section-animate" style="background:var(--off-white);padding:80px 24px;">
  <div style="max-width:1000px;margin:0 auto;">
    <p style="font-family:var(--font-inter);font-size:0.75rem;font-weight:600;letter-spacing:0.1em;color:var(--gold);text-transform:uppercase;margin-bottom:12px;">EDUCATION</p>
    <h2 style="font-family:var(--font-playfair);font-size:clamp(1.75rem,4vw,2.5rem);color:var(--navy);margin-bottom:40px;">Academic Foundation</h2>
    <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:24px;">
      {#each education as edu}
        <article style="background:white;border:1px solid var(--highlight);border-radius:16px;padding:28px;box-shadow:var(--shadow-card);">
          <div style="display:flex;align-items:flex-start;gap:16px;margin-bottom:20px;">
            <img
              src="{base}/images/{edu.logo}"
              alt="Gies College of Business logo"
              width="56"
              height="56"
              loading="lazy"
              style="border-radius:10px;border:1px solid var(--highlight);object-fit:contain;padding:6px;background:white;flex-shrink:0;"
            />
            <div>
              <h3 style="font-family:var(--font-playfair);font-size:1.0625rem;font-weight:600;color:var(--navy);line-height:1.3;">{edu.degree}</h3>
              <p style="font-family:var(--font-inter);font-size:0.8125rem;color:var(--muted);margin-top:4px;">{edu.school}</p>
            </div>
          </div>
          <div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:8px;margin-bottom:16px;">
            <span style="font-family:var(--font-inter);font-size:0.8125rem;color:var(--muted);">{edu.period}</span>
          </div>
          {#if edu.honors.length > 0}
            <div style="margin-bottom:12px;display:flex;gap:8px;flex-wrap:wrap;">
              {#each edu.honors as honor}
                <span style="font-family:var(--font-inter);font-size:0.75rem;font-weight:600;color:var(--gold-dark);background:#fefbf0;border:1px solid var(--gold-light);padding:3px 10px;border-radius:99px;">{honor}</span>
              {/each}
            </div>
          {/if}
          <p style="font-family:var(--font-inter);font-size:0.8125rem;color:var(--muted);">{edu.concentrations.join(' · ')}</p>
        </article>
      {/each}
    </div>
  </div>
</section>
