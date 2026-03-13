<script lang="ts">
  import { onMount } from 'svelte';

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

  const highlights = [
    { title: 'U.S. GAAP Taxonomy', sub: 'FASB XBRL Postgraduate Technical Assistant' },
    { title: 'Dual 4.0 GPA', sub: 'BS & MAS · Gies College of Business, UIUC' },
    { title: 'CPA Licensed', sub: 'All exam sections passed · 2025' },
  ];
</script>

<section id="about" bind:this={sectionEl} class="section-animate" style="background:var(--off-white);padding:80px 24px;">
  <div style="max-width:1100px;margin:0 auto;">
    <p style="font-family:var(--font-inter);font-size:0.75rem;font-weight:600;letter-spacing:0.1em;color:var(--gold);text-transform:uppercase;margin-bottom:12px;">ABOUT</p>
    <h2 style="font-family:var(--font-playfair);font-size:clamp(1.75rem,4vw,2.5rem);color:var(--navy);margin-bottom:40px;">Where precision meets purpose.</h2>
    <div style="display:grid;grid-template-columns:1fr;gap:40px;">
      <div>
        <p style="font-family:var(--font-inter);font-size:1rem;color:var(--ink);line-height:1.8;margin-bottom:16px;">
          I studied accountancy at the University of Illinois Urbana-Champaign's Gies College of Business, earning both my Bachelor's and Master's degrees with concentrations in Financial Reporting &amp; Assurance and Data Analytics — graduating with a perfect 4.0 in both programs.
        </p>
        <p style="font-family:var(--font-inter);font-size:1rem;color:var(--ink);line-height:1.8;margin-bottom:16px;">
          I'm currently the 2025–2026 XBRL Postgraduate Technical Assistant at the Financial Accounting Standards Board (FASB) in Norwalk, Connecticut, where I support the development and maintenance of the U.S. GAAP Taxonomy, contribute to intangibles research, and participate in the Public Markets Advisory Committee (PMAC).
        </p>
        <p style="font-family:var(--font-inter);font-size:1rem;color:var(--ink);line-height:1.8;">
          My career spans audit, competitive intelligence, data analytics, and financial standards — working across Caterpillar Inc., UIUC, and FASB. I hold CPA licensure with all exam sections passed in 2025.
        </p>
      </div>
      <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:16px;">
        {#each highlights as card}
          <div style="background:white;border:1px solid var(--highlight);border-left:3px solid var(--gold);border-radius:12px;padding:20px 24px;box-shadow:var(--shadow-card);">
            <h3 style="font-family:var(--font-playfair);font-size:1.125rem;color:var(--navy);font-weight:600;margin-bottom:6px;">{card.title}</h3>
            <p style="font-family:var(--font-inter);font-size:0.875rem;color:var(--muted);">{card.sub}</p>
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
