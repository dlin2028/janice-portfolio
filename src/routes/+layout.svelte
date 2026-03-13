<script lang="ts">
  import '../app.css';

  let { children } = $props();

  const personSchema = {
    '@context': 'https://schema.org',
    '@type': 'Person',
    name: 'Janice Jiang',
    url: 'https://dlin2028.github.io/janice-portfolio',
    email: 'jjiang@fasb.org',
    image: 'https://dlin2028.github.io/janice-portfolio/images/profile.jpg',
    jobTitle: 'Postgraduate Technical Assistant',
    worksFor: {
      '@type': 'Organization',
      name: 'Financial Accounting Standards Board (FASB)',
      url: 'https://www.fasb.org',
    },
    alumniOf: [
      {
        '@type': 'EducationalOrganization',
        name: 'Gies College of Business, University of Illinois Urbana-Champaign',
        url: 'https://giesbusiness.illinois.edu',
      },
    ],
    sameAs: ['https://www.linkedin.com/in/janice-jiang-508bba21b/'],
    knowsAbout: ['XBRL', 'U.S. GAAP', 'Financial Reporting', 'Data Analytics', 'Python'],
    hasCredential: {
      '@type': 'EducationalOccupationalCredential',
      credentialCategory: 'Certified Public Accountant (CPA)',
    },
    address: {
      '@type': 'PostalAddress',
      addressLocality: 'Norwalk',
      addressRegion: 'CT',
      addressCountry: 'US',
    },
  };
</script>

<svelte:head>
  <title>Janice Jiang — XBRL Specialist & CPA | FASB</title>
  <meta name="description" content="Janice Jiang is the 2025–2026 XBRL Postgraduate Technical Assistant at FASB, contributing to the U.S. GAAP Taxonomy. CPA. Gies College of Business, UIUC. Dual 4.0 GPA." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://dlin2028.github.io/janice-portfolio" />
  <meta property="og:site_name" content="Janice Jiang" />
  <meta property="og:title" content="Janice Jiang — XBRL Specialist & CPA | FASB" />
  <meta property="og:description" content="Postgraduate Technical Assistant at FASB, building the U.S. GAAP Taxonomy. CPA | Gies UIUC | 4.0 GPA." />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Janice Jiang — XBRL Specialist & CPA | FASB" />
  <meta name="twitter:description" content="Postgraduate Technical Assistant at FASB, building the U.S. GAAP Taxonomy. CPA | Gies UIUC | 4.0 GPA." />
  <meta name="robots" content="index,follow,max-snippet:-1,max-image-preview:large" />
  {@html `<script type="application/ld+json">${JSON.stringify(personSchema)}</script>`}
</svelte:head>

{@render children()}
