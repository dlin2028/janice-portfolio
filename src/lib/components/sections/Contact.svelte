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
</script>

<section id="contact" bind:this={sectionEl} class="section-animate" style="background:var(--off-white);padding:80px 24px;">
  <div style="max-width:600px;margin:0 auto;text-align:center;">
    <p style="font-family:var(--font-inter);font-size:0.75rem;font-weight:600;letter-spacing:0.1em;color:var(--gold);text-transform:uppercase;margin-bottom:12px;">CONTACT</p>
    <h2 style="font-family:var(--font-playfair);font-size:clamp(1.75rem,4vw,2.5rem);color:var(--navy);margin-bottom:20px;">Let's Connect.</h2>
    <p style="font-family:var(--font-inter);font-size:1rem;color:var(--muted);line-height:1.8;margin-bottom:32px;">
      I'm open to conversations about financial reporting, XBRL, accounting standards, and opportunities at the intersection of accounting and data. The best way to reach me is email.
    </p>
    <div style="display:flex;flex-direction:column;align-items:center;gap:16px;">
      <a
        href="mailto:jjiang@fasb.org"
        style="font-family:var(--font-inter);font-size:1.125rem;font-weight:600;color:var(--navy);text-decoration:none;border-bottom:2px solid var(--gold);padding-bottom:2px;transition:color 0.2s;"
        onmouseenter={(e) => { (e.currentTarget as HTMLElement).style.color='var(--gold)'; }}
        onmouseleave={(e) => { (e.currentTarget as HTMLElement).style.color='var(--navy)'; }}
      >
        jjiang@fasb.org
      </a>
      <a
        href="https://www.linkedin.com/in/janice-jiang-508bba21b/"
        target="_blank"
        rel="noopener noreferrer"
        style="font-family:var(--font-inter);font-size:0.9375rem;font-weight:500;color:var(--navy);text-decoration:none;border:1.5px solid var(--navy);border-radius:6px;padding:10px 24px;transition:all 0.2s;"
        onmouseenter={(e) => { const el = e.currentTarget as HTMLElement; el.style.background='var(--navy)'; el.style.color='white'; }}
        onmouseleave={(e) => { const el = e.currentTarget as HTMLElement; el.style.background='transparent'; el.style.color='var(--navy)'; }}
      >
        View LinkedIn Profile →
      </a>
    </div>
    <p style="font-family:var(--font-inter);font-size:0.8125rem;color:var(--muted);margin-top:32px;">
      Norwalk, Connecticut · Open to professional inquiries
    </p>
  </div>
</section>

<footer style="background:var(--navy-dark);padding:24px;text-align:center;">
  <p style="font-family:var(--font-inter);font-size:0.8125rem;color:rgba(255,255,255,0.4);">
    © {new Date().getFullYear()} Janice Jiang
  </p>
</footer>
