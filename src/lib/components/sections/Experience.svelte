<script lang="ts">
  import { onMount } from 'svelte';
  import { base } from '$app/paths';
  import { experience } from '$lib/data/experience.js';

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

<section id="experience" bind:this={sectionEl} class="section-animate" style="background:white;padding:80px 24px;">
  <div style="max-width:900px;margin:0 auto;">
    <p style="font-family:var(--font-inter);font-size:0.75rem;font-weight:600;letter-spacing:0.1em;color:var(--gold);text-transform:uppercase;margin-bottom:12px;">EXPERIENCE</p>
    <h2 style="font-family:var(--font-playfair);font-size:clamp(1.75rem,4vw,2.5rem);color:var(--navy);margin-bottom:40px;">Where I've Worked</h2>
    <div style="display:flex;flex-direction:column;gap:24px;">
      {#each experience as exp}
        <article style="background:white;border:1px solid var(--highlight);border-radius:16px;padding:24px;box-shadow:var(--shadow-card);transition:all 0.25s;"
          onmouseenter={(e) => { const el = e.currentTarget as HTMLElement; el.style.boxShadow='var(--shadow-hover)'; el.style.transform='translateY(-2px)'; }}
          onmouseleave={(e) => { const el = e.currentTarget as HTMLElement; el.style.boxShadow='var(--shadow-card)'; el.style.transform='translateY(0)'; }}
        >
          <div style="display:flex;align-items:flex-start;gap:16px;margin-bottom:16px;">
            <img
              src="{base}/images/{exp.logo}"
              alt="{exp.company} logo"
              width="56"
              height="56"
              loading="lazy"
              style="border-radius:10px;border:1px solid var(--highlight);object-fit:contain;padding:6px;background:white;flex-shrink:0;"
            />
            <div>
              <h3 style="font-family:var(--font-playfair);font-size:1rem;font-weight:600;color:var(--navy);">{exp.company}</h3>
              <p style="font-family:var(--font-inter);font-size:0.875rem;color:var(--muted);margin-top:2px;">{exp.location}</p>
            </div>
          </div>
          <div style="display:flex;flex-direction:column;gap:16px;">
            {#each exp.roles as role, i}
              <div style="{i > 0 ? 'padding-top:16px;border-top:1px solid var(--highlight)' : ''}">
                <div style="display:flex;align-items:baseline;justify-content:space-between;gap:16px;margin-bottom:8px;flex-wrap:wrap;">
                  <p style="font-family:var(--font-inter);font-size:0.9375rem;font-weight:600;color:var(--ink);">{role.title}</p>
                  <p style="font-family:var(--font-inter);font-size:0.75rem;color:var(--muted);white-space:nowrap;">{role.period}</p>
                </div>
                {#if role.bullets.length > 0}
                  <ul style="list-style:none;padding:0;margin:0;display:flex;flex-direction:column;gap:6px;">
                    {#each role.bullets as bullet}
                      <li style="display:flex;gap:8px;font-family:var(--font-inter);font-size:0.875rem;color:var(--ink);line-height:1.6;">
                        <span style="color:var(--gold);margin-top:2px;flex-shrink:0;">•</span>
                        {bullet}
                      </li>
                    {/each}
                  </ul>
                {/if}
              </div>
            {/each}
          </div>
        </article>
      {/each}
    </div>
  </div>
</section>
