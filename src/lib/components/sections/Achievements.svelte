<script lang="ts">
  import { achievements } from '$lib/data/achievements.js';
</script>

<section id="achievements" style="background:var(--navy);padding:64px 24px;">
  <div style="max-width:1200px;margin:0 auto;display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:2px;">
    {#each achievements as tile}
      <div style="text-align:center;padding:32px 24px;border-right:1px solid rgba(255,255,255,0.08);">
        <p style="font-family:var(--font-playfair);font-size:clamp(1.75rem,4vw,2.5rem);font-weight:700;color:var(--gold);line-height:1.1;margin-bottom:8px;">{tile.callout}</p>
        <p style="font-family:var(--font-playfair);font-size:1rem;font-weight:600;color:white;margin-bottom:6px;">{tile.title}</p>
        <p style="font-family:var(--font-inter);font-size:0.8125rem;color:rgba(255,255,255,0.6);">{tile.sub}</p>
      </div>
    {/each}
  </div>
</section>
