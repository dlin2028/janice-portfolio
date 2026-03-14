<script lang="ts">
  import { onMount } from 'svelte';

  const links = [
    { href: '#about', label: 'About' },
    { href: '#experience', label: 'Experience' },
    { href: '#education', label: 'Education' },
    { href: '#skills', label: 'Skills' },
    { href: '#contact', label: 'Contact' },
  ];

  let scrolled = $state(false);
  let menuOpen = $state(false);

  onMount(() => {
    const handler = () => { scrolled = window.scrollY > 80; };
    window.addEventListener('scroll', handler, { passive: true });
    return () => window.removeEventListener('scroll', handler);
  });

  function closeMenu() { menuOpen = false; }
</script>

<nav
  style="position:fixed;top:0;left:0;right:0;z-index:50;height:72px;display:flex;align-items:center;transition:all 0.3s;{scrolled ? 'background:white;box-shadow:0 1px 8px rgba(0,0,0,0.08)' : 'background:transparent'}"
  aria-label="Main navigation"
>
  <div style="max-width:1100px;margin:0 auto;width:100%;padding:0 24px;display:flex;align-items:center;justify-content:space-between;">
    <span style="font-family:var(--font-playfair);font-weight:500;font-size:1.125rem;{scrolled ? 'color:var(--navy)' : 'color:white'}">
      Janice Jiang
    </span>
    <ul style="display:flex;align-items:center;gap:32px;list-style:none;margin:0;padding:0;" role="list">
      {#each links as link}
        <li>
          <a
            href={link.href}
            onclick={closeMenu}
            style="font-family:var(--font-inter);font-size:0.875rem;font-weight:500;text-decoration:none;transition:color 0.2s;position:relative;{scrolled ? 'color:var(--muted)' : 'color:rgba(255,255,255,0.9)'}"
            class="nav-link"
            onmouseenter={(e) => { (e.currentTarget as HTMLElement).style.color = 'var(--gold)'; }}
            onmouseleave={(e) => { (e.currentTarget as HTMLElement).style.color = scrolled ? 'var(--muted)' : 'rgba(255,255,255,0.9)'; }}
          >
            {link.label}
          </a>
        </li>
      {/each}
    </ul>
    <a
      href="#contact"
      style="font-family:var(--font-inter);font-size:0.875rem;font-weight:500;text-decoration:none;border-radius:9999px;padding:8px 20px;transition:all 0.2s;{scrolled ? 'border:1.5px solid var(--navy);color:var(--navy)' : 'border:1.5px solid white;color:white'}"
      onmouseenter={(e) => { const el = e.currentTarget as HTMLElement; if (scrolled) { el.style.background='var(--navy)'; el.style.color='white'; } else { el.style.background='rgba(255,255,255,0.1)'; } }}
      onmouseleave={(e) => { const el = e.currentTarget as HTMLElement; el.style.background='transparent'; if (scrolled) { el.style.color='var(--navy)'; } else { el.style.color='white'; } }}
    >
      Contact
    </a>
  </div>
</nav>
