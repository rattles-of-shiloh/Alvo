<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Portfolio of Maya Lin — Product Design & Human-Computer Interaction Student showcasing academic research, digital products, and creative systems." />
  <meta name="author" content="Maya Lin" />
  <meta name="theme-color" content="#FAF8F5" />
  <title>Maya Lin — Product Design & HCI Portfolio</title>

  <!-- Inline SVG Favicon Placeholder -->
  <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://w3.org' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='12' fill='%23141413'/%3E%3Ctext x='50%25' y='54%25' dominant-baseline='middle' text-anchor='middle' font-family='Georgia, serif' font-style='italic' font-weight='bold' font-size='32' fill='%23FAF8F5'%3EM%3C/text%3E%3C/svg%3E" />

  <!-- Google Fonts Pairing: Playfair Display + Plus Jakarta Sans + JetBrains Mono -->
  <link rel="preconnect" href="https://googleapis.com" />
  <link rel="preconnect" href="https://gstatic.com" crossorigin />
  <link href="https://googleapis.com/css2?family=JetBrains+Mono:wght@400;500&family=Playfair+Display:ital,wght@0,500;0,700;0,800;1,500;1,700&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet" />

  <style>
    /* =========================================
       1. DESIGN TOKENS & EDITORIAL PALETTE
       ========================================= */
    :root {
      --bg-primary: #FAF8F5;       /* Warm Editorial Paper */
      --bg-secondary: #F2EFE9;     /* Subtle Cream Contrast */
      --bg-card: #FFFFFF;          /* Crisp Card Surface */
      --ink-primary: #141413;      /* Rich Charcoal Ink */
      --ink-secondary: #52504C;    /* Muted Editorial Gray */
      --ink-muted: #85827C;        /* Caption & Meta Gray */
      --accent: #C84B31;           /* Terracotta Print Accent */
      --accent-hover: #A83A23;     /* Deep Terracotta */
      --border-hairline: #DED9D0;  /* Fine Magazine Rule */
      --border-strong: #141413;    /* Bold Editorial Divider */

      --font-serif: 'Playfair Display', Georgia, serif;
      --font-sans: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif;
      --font-mono: 'JetBrains Mono', monospace;

      --container-max: 1220px;
      --gutter: clamp(1.25rem, 4vw, 3rem);
      --section-pad: clamp(4.5rem, 8vw, 7.5rem);
      --transition: 0.35s cubic-bezier(0.22, 1, 0.36, 1);
    }

    /* =========================================
       2. RESET & BASE TYPOGRAPHY
       ========================================= */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      font-size: 16px;
      scroll-behavior: smooth;
      background-color: var(--bg-primary);
      color: var(--ink-primary);
    }

    body {
      font-family: var(--font-sans);
      line-height: 1.65;
      color: var(--ink-primary);
      background-color: var(--bg-primary);
      -webkit-font-smoothing: antialiased;
      overflow-x: hidden;
    }

    img, svg {
      display: block;
      max-width: 100%;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    ::selection {
      background-color: var(--accent);
      color: #FFFFFF;
    }

    .container {
      width: 100%;
      max-width: var(--container-max);
      margin: 0 auto;
      padding-left: var(--gutter);
      padding-right: var(--gutter);
    }

    /* Editorial Section Header Pattern */
    .section-header {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: baseline;
      gap: 1rem;
      padding-bottom: 1.25rem;
      margin-bottom: clamp(2.5rem, 5vw, 3.75rem);
      border-bottom: 2px solid var(--border-strong);
    }

    .section-eyebrow {
      font-family: var(--font-mono);
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.14em;
      color: var(--accent);
      font-weight: 500;
    }

    .section-title {
      font-family: var(--font-serif);
      font-size: clamp(2.1rem, 4vw, 3.1rem);
      font-weight: 700;
      line-height: 1.1;
      letter-spacing: -0.02em;
    }

    /* =========================================
       3. STICKY MINIMAL HEADER
       ========================================= */
    .site-header {
      position: sticky;
      top: 0;
      z-index: 100;
      background-color: rgba(250, 248, 245, 0.92);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border-hairline);
      transition: box-shadow var(--transition);
    }

    .site-header.scrolled {
      box-shadow: 0 4px 24px rgba(20, 20, 19, 0.04);
    }

    .nav-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 4.5rem;
    }

    .brand-mark {
      display: flex;
      align-items: center;
      gap: 0.65rem;
      font-family: var(--font-serif);
      font-weight: 700;
      font-size: 1.25rem;
      letter-spacing: -0.01em;
    }

    .brand-dot {
      width: 9px;
      height: 9px;
      border-radius: 50%;
      background-color: var(--accent);
      display: inline-block;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: clamp(1rem, 2.5vw, 2.25rem);
      list-style: none;
    }

    .nav-links a {
      font-size: 0.88rem;
      font-weight: 500;
      color: var(--ink-secondary);
      position: relative;
      padding: 0.25rem 0;
      transition: color 0.2s ease;
    }

    .nav-links a::after {
      content: "";
      position: absolute;
      left: 0;
      bottom: 0;
      width: 0;
      height: 1.5px;
      background-color: var(--accent);
      transition: width var(--transition);
    }

    .nav-links a:hover,
    .nav-links a.active {
      color: var(--ink-primary);
    }

    .nav-links a:hover::after,
    .nav-links a.active::after {
      width: 100%;
    }

    .nav-cta {
      font-family: var(--font-mono);
      font-size: 0.78rem;
      padding: 0.55rem 1.1rem;
      border: 1px solid var(--ink-primary);
      border-radius: 999px;
      transition: all 0.25s ease;
    }

    .nav-cta:hover {
      background-color: var(--ink-primary);
      color: var(--bg-primary);
    }

    /* =========================================
       4. SPLIT-SCREEN HERO SECTION
       ========================================= */
    .hero {
      border-bottom: 1px solid var(--border-hairline);
      padding-top: clamp(2.5rem, 5vw, 4rem);
      padding-bottom: clamp(3.5rem, 6vw, 5.5rem);
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.15fr 0.85fr;
      gap: clamp(2.5rem, 5vw, 4.5rem);
      align-items: center;
    }

    .hero-meta {
      display: inline-flex;
      align-items: center;
      gap: 0.75rem;
      font-family: var(--font-mono);
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      color: var(--ink-secondary);
      margin-bottom: 1.5rem;
      padding-bottom: 0.65rem;
      border-bottom: 1px solid var(--border-hairline);
    }

    .status-pill {
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      color: var(--accent);
      font-weight: 500;
    }

    .status-pill::before {
      content: "";
      width: 7px;
      height: 7px;
      border-radius: 50%;
      background-color: var(--accent);
    }

    .hero-name {
      font-family: var(--font-serif);
      font-size: clamp(3.25rem, 6.5vw, 5.4rem);
      font-weight: 800;
      line-height: 1.02;
      letter-spacing: -0.03em;
      margin-bottom: 1.5rem;
    }

    .hero-name em {
      font-style: italic;
      font-weight: 500;
      color: var(--accent);
    }

    .hero-tagline {
      font-size: clamp(1.125rem, 1.8vw, 1.35rem);
      color: var(--ink-secondary);
      max-width: 34ch;
      line-height: 1.55;
      margin-bottom: 2.25rem;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 1.25rem;
    }

    .btn-primary {
      display: inline-flex;
      align-items: center;
      gap: 0.65rem;
      background-color: var(--ink-primary);
      color: var(--bg-primary);
      font-weight: 600;
      font-size: 0.95rem;
      padding: 1rem 1.85rem;
      border-radius: 2px;
      border: 1px solid var(--ink-primary);
      transition: all var(--transition);
    }

    .btn-primary:hover {
      background-color: var(--accent);
      border-color: var(--accent);
      transform: translateY(-2px);
    }

    .btn-secondary {
      font-family: var(--font-mono);
      font-size: 0.82rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--ink-primary);
      border-bottom: 1px solid var(--ink-primary);
      padding-bottom: 0.2rem;
      transition: color 0.2s ease, border-color 0.2s ease;
    }

    .btn-secondary:hover {
      color: var(--accent);
      border-color: var(--accent);
    }

    /* Split Hero Right Visual Frame */
    .hero-visual {
      position: relative;
    }

    .portrait-frame {
      position: relative;
      aspect-ratio: 4 / 5;
      background-color: var(--bg-secondary);
      border: 1px solid var(--border-strong);
      padding: 0.85rem;
      box-shadow: 14px 14px 0px var(--bg-secondary), 14px 14px 0px 1px var(--border-hairline);
    }

    .portrait-placeholder {
      width: 100%;
      height: 100%;
      background: linear-gradient(145deg, #E7E1D6 0%, #D4CBBF 100%);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      padding: 1.75rem;
      position: relative;
      overflow: hidden;
    }

    .portrait-caption {
      display: flex;
      justify-content: space-between;
      font-family: var(--font-mono);
      font-size: 0.72rem;
      text-transform: uppercase;
