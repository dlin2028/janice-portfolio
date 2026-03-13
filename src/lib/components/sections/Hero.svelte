<script lang="ts">
</script>

<section id="hero" style="min-height:100vh;background:linear-gradient(135deg,var(--navy) 0%,var(--navy-light) 100%);display:flex;align-items:center;justify-content:center;padding:120px 24px 80px;position:relative;overflow:hidden;">
  <div style="max-width:900px;width:100%;margin:0 auto;display:flex;flex-direction:column;align-items:center;text-align:center;gap:24px;">
    <div style="width:160px;height:160px;border-radius:50%;overflow:hidden;border:3px solid rgba(255,255,255,0.8);box-shadow:0 8px 32px rgba(0,0,0,0.3);flex-shrink:0;">
      <img
        src="/images/profile.jpg"
        alt="Janice Jiang — Postgraduate Technical Assistant at FASB"
        width="160"
        height="160"
        loading="eager"
        style="width:100%;height:100%;object-fit:cover;"
      />
    </div>
    <div>
      <h1 style="font-family:var(--font-playfair);font-weight:700;font-size:clamp(2.5rem,6vw,4.5rem);color:white;line-height:1.1;margin-bottom:8px;">
        Janice Jiang
        <span style="display:block;width:80px;height:3px;background:var(--gold);margin:12px auto 0;"></span>
      </h1>
      <p style="font-family:var(--font-inter);font-size:clamp(1rem,2.5vw,1.375rem);color:rgba(255,255,255,0.9);margin-top:16px;font-weight:500;">
        Postgraduate Technical Assistant · FASB
      </p>
      <p style="font-family:var(--font-inter);font-size:1rem;color:rgba(255,255,255,0.7);margin-top:6px;">
        CPA · Gies UIUC · 4.0 GPA
      </p>
      <p style="font-family:var(--font-inter);font-size:1.0625rem;color:rgba(255,255,255,0.85);margin-top:16px;font-style:italic;">
        Building the infrastructure of U.S. financial reporting.
      </p>
    </div>
    <div style="display:flex;gap:16px;flex-wrap:wrap;justify-content:center;margin-top:8px;">
      <a
        href="#experience"
        style="font-family:var(--font-inter);font-size:0.9375rem;font-weight:600;text-decoration:none;background:var(--gold);color:var(--navy-dark);padding:12px 28px;border-radius:6px;transition:all 0.2s;display:inline-block;"
        onmouseenter={(e) => { (e.currentTarget as HTMLElement).style.background='var(--gold-light)'; }}
        onmouseleave={(e) => { (e.currentTarget as HTMLElement).style.background='var(--gold)'; }}
      >
        View My Work
      </a>
      <a
        href="#contact"
        style="font-family:var(--font-inter);font-size:0.9375rem;font-weight:600;text-decoration:none;border:2px solid rgba(255,255,255,0.7);color:white;padding:12px 28px;border-radius:6px;transition:all 0.2s;display:inline-block;"
        onmouseenter={(e) => { (e.currentTarget as HTMLElement).style.background='rgba(255,255,255,0.1)'; }}
        onmouseleave={(e) => { (e.currentTarget as HTMLElement).style.background='transparent'; }}
      >
        Get In Touch
      </a>
    </div>
  </div>
</section>
