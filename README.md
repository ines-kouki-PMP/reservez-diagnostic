<!DOCTYPE html>
<html lang="fr" style="color-scheme: dark;">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#2E1F47">
<title>Inès Kouki — Diagnostic R.P.T. · Rôle · Posture · Trajectoire</title>
<meta name="description" content="Clarifiez votre rôle réel, renforcer votre posture et piloter votre trajectoire dans des organisations complexes. 17 ans en transformation. Afrique, Europe.">
<meta property="og:title" content="Inès Kouki — Diagnostic R.P.T.">
<meta property="og:description" content="De la confusion professionnelle à la clarté stratégique. Rôle · Posture · Trajectoire.">
<meta property="og:type" content="website">
<link rel="canonical" href="https://ineskouki.com">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500&family=EB+Garamond:ital,wght@1,400;1,500;1,600&display=swap" rel="stylesheet">

<style>
:root {
  /* Palette violet nuit + crème — identité de marque Ines Kouki */
  --midnight:        #1C1030;
  --deep-violet:     #2E1F47;
  --violet-mid:      #3A2856;
  --slate:           #5A4878;
  --slate-light:     #7B6AA0;
  --cream:           #FAF7F2;
  --ivory:           #F5F0E8;
  --pearl:           #E8DFD2;
  --warm-gray:       #C0B6D0;
  --warm-gray-light: #D4CCDF;
  --terracotta:      #C4789A;
  --terracotta-deep: #A85F80;
  --terracotta-pale: #E8B4CC;
  --teal:            #4B7F8C;
  --sage:            #6B8068;
  --gold:            #C9A96E;

  --display: "Playfair Display", Georgia, serif;
  --body:    "Plus Jakarta Sans", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  --mono:    "JetBrains Mono", monospace;

  --radius-sm: 4px;
  --radius-md: 8px;
  --shadow-card: 0 4px 40px rgba(0,0,0,0.35);
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }

body {
  background: var(--midnight);
  color: var(--cream);
  font-family: var(--body);
  font-size: 19px;
  line-height: 1.7;
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
  overflow-x: hidden;
}

/* Grain texture overlay */
body::before {
  content: "";
  position: fixed; inset: 0;
  pointer-events: none; z-index: 1;
  opacity: 0.04;
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='200' height='200'><filter id='n'><feTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='3'/></filter><rect width='200' height='200' filter='url(%23n)'/></svg>");
}

.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
}

a { color: inherit; text-decoration: none; }
a:focus-visible, button:focus-visible { outline: 2px solid var(--terracotta); outline-offset: 3px; }
button, a { touch-action: manipulation; -webkit-tap-highlight-color: transparent; }

/* ─── FADE-IN ANIMATIONS ─── */
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(28px); }
  to   { opacity: 1; transform: translateY(0); }
}
@keyframes fadeIn {
  from { opacity: 0; }
  to   { opacity: 1; }
}
@keyframes lineGrow {
  from { transform: scaleX(0); }
  to   { transform: scaleX(1); }
}
@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50%       { transform: translateY(-8px); }
}

.fade-up {
  opacity: 0;
  animation: fadeUp 0.75s cubic-bezier(0.22,1,0.36,1) forwards;
}
.fade-up.d1 { animation-delay: 0.1s; }
.fade-up.d2 { animation-delay: 0.25s; }
.fade-up.d3 { animation-delay: 0.4s; }
.fade-up.d4 { animation-delay: 0.55s; }
.fade-up.d5 { animation-delay: 0.7s; }

/* ─── NAV ─── */
.nav {
  position: fixed; top: 0; left: 0; right: 0;
  z-index: 100;
  padding: 0;
  background: rgba(28, 16, 48, 0.85);
  backdrop-filter: blur(20px) saturate(140%);
  border-bottom: 1px solid rgba(232, 223, 210, 0.08);
  transition: all 0.4s ease;
}

.nav-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 40px;
  max-width: 1200px;
  margin: 0 auto;
}

.logo {
  font-family: var(--display);
  font-size: 24px;
  font-weight: 500;
  letter-spacing: 0.06em;
  color: var(--cream);
}

.logo span {
  color: var(--terracotta);
  font-style: normal;
  font-weight: 600;
}

.nav-tag {
  font-family: var(--mono);
  font-size: 14px;
  letter-spacing: 0.08em;
  color: var(--warm-gray);
  text-transform: uppercase;
}

/* ─── HERO ─── */
.hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  padding: 140px 0 80px;
  overflow: hidden;
}

/* Ambient orbs */
.hero::before {
  content: "";
  position: absolute;
  top: -100px; left: 50%; transform: translateX(-60%);
  width: 700px; height: 700px;
  background: radial-gradient(ellipse, rgba(196,120,154,0.12) 0%, transparent 65%);
  pointer-events: none;
}
.hero::after {
  content: "";
  position: absolute;
  bottom: -50px; right: -100px;
  width: 500px; height: 500px;
  background: radial-gradient(ellipse, rgba(75,127,140,0.1) 0%, transparent 65%);
  pointer-events: none;
}

.hero-content {
  text-align: center;
  max-width: 900px;
  margin: 0 auto;
  position: relative; z-index: 2;
}

.hero-label {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  padding: 8px 20px;
  border: 1px solid rgba(196, 120, 154, 0.3);
  background: rgba(196, 120, 154, 0.08);
  font-family: var(--mono);
  font-size: 14px;
  letter-spacing: 0.10em;
  text-transform: uppercase;
  color: var(--terracotta-pale);
  margin-bottom: 40px;
}

.hero-label::before {
  content: "";
  width: 6px; height: 6px;
  border-radius: 50%;
  background: var(--terracotta);
  animation: float 2.5s ease-in-out infinite;
}

.hero h1 {
  font-family: var(--display);
  font-size: clamp(36px, 7.5vw, 80px);
  font-weight: 400;
  line-height: 1.12;
  letter-spacing: -0.02em;
  margin-bottom: 32px;
  color: var(--cream);
}

.hero h1 em {
  color: var(--terracotta);
  font-style: italic;
}

.hero-sub {
  font-size: 20px;
  color: var(--warm-gray);
  max-width: 680px;
  margin: 0 auto 16px;
  line-height: 1.75;
}

.hero-sub strong {
  color: var(--cream);
  font-weight: 500;
}

.hero-divider {
  width: 60px; height: 1px;
  background: linear-gradient(90deg, transparent, var(--terracotta), transparent);
  margin: 28px auto;
}

.hero-promise {
  font-size: 22px;
  color: var(--warm-gray-light);
  font-style: italic;
  font-family: var(--body);
  font-weight: 400;
  margin-bottom: 40px;
}

.hero-cta-group {
  display: flex;
  gap: 16px;
  justify-content: center;
  flex-wrap: wrap;
}

.cta-with-badge {
  position: relative;
  overflow: visible !important;
}
.cta-with-badge {
  position: relative !important;
}
.cta-with-badge .cta-badge {
  position: absolute;
  top: -14px;
  right: 18px;
  display: inline-block;
  background: var(--cream);
  color: var(--midnight);
  font-family: var(--mono);
  font-size: 9px;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  font-weight: 700;
  padding: 3px 10px;
  border-radius: 999px;
  white-space: nowrap;
  animation: cta-badge-float 2.4s ease-in-out infinite;
  box-shadow:
    0 4px 14px rgba(196, 120, 154, 0.40),
    0 0 0 1.5px rgba(196, 120, 154, 0.25);
}
@keyframes cta-badge-float {
  0%, 100% { transform: translateY(0) rotate(-2deg); }
  50% { transform: translateY(-4px) rotate(-2deg); }
}
@media (prefers-reduced-motion: reduce) {
  .cta-with-badge .cta-badge { animation: none; }
}
.discovery-cta {
  display: inline-flex;
  align-items: center;
  margin-top: 24px;
}

.btn-primary {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 16px 40px;
  min-height: 52px;
  background: var(--terracotta);
  color: var(--midnight);
  font-weight: 600;
  font-size: 17px;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  border: none;
  cursor: pointer;
  transition: all 0.3s cubic-bezier(0.22,1,0.36,1);
  position: relative;
  overflow: hidden;
}

.btn-primary::after {
  content: "";
  position: absolute; inset: 0;
  background: rgba(255,255,255,0.15);
  transform: translateX(-100%);
  transition: transform 0.4s ease;
}

.btn-primary:hover { background: var(--terracotta-deep); transform: translateY(-2px); box-shadow: 0 8px 30px rgba(196,120,154,0.35); }
.btn-primary:hover::after { transform: translateX(0); }

.btn-ghost {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 16px 32px;
  min-height: 52px;
  background: transparent;
  color: var(--warm-gray-light);
  font-size: 17px;
  letter-spacing: 0.04em;
  border: 1px solid rgba(232,223,210,0.15);
  cursor: pointer;
  transition: all 0.3s ease;
}
.btn-ghost:hover { border-color: rgba(196,120,154,0.4); color: var(--cream); }

.hero-scroll {
  position: absolute;
  bottom: 40px; left: 50%; transform: translateX(-50%);
  display: flex; flex-direction: column; align-items: center; gap: 8px;
  font-family: var(--mono); font-size: 10px; letter-spacing: 0.12em;
  color: var(--warm-gray); text-transform: uppercase; z-index: 2;
}
.scroll-line {
  width: 1px; height: 40px;
  background: linear-gradient(180deg, var(--terracotta) 0%, transparent 100%);
  animation: float 2s ease-in-out infinite;
}

/* ─── MARQUEE STRIP ─── */
.marquee-strip {
  overflow: hidden;
  border-top: 1px solid rgba(232,223,210,0.08);
  border-bottom: 1px solid rgba(232,223,210,0.08);
  padding: 16px 0;
  background: rgba(58, 40, 86, 0.3);
}
.marquee-track {
  display: flex;
  gap: 48px;
  animation: marquee 22s linear infinite;
  width: max-content;
}
@keyframes marquee { from { transform: translateX(0); } to { transform: translateX(-50%); } }
.marquee-item {
  font-family: var(--mono);
  font-size: 14px;
  letter-spacing: 0.14em;
  color: var(--warm-gray);
  text-transform: uppercase;
  white-space: nowrap;
  display: flex; align-items: center; gap: 16px;
}
.marquee-item::after { content: "·"; color: var(--terracotta); }

/* ─── DISCOVERY CALL ─── */
.discovery {
  padding: 80px 0;
  border-bottom: 1px solid rgba(232,223,210,0.08);
}
.discovery-inner {
  text-align: center;
  max-width: 680px;
  margin: 0 auto;
  padding: 56px 48px;
  border: 1px solid rgba(232,223,210,0.12);
  background: rgba(58,40,86,0.35);
  position: relative;
}
.discovery-inner::before {
  content: "";
  position: absolute; top: 0; left: 50%; transform: translateX(-50%);
  width: 60px; height: 2px;
  background: var(--terracotta);
}
.discovery-inner h2 {
  font-family: var(--display);
  font-size: 38px; font-weight: 400;
  margin-bottom: 16px;
  letter-spacing: -0.01em;
}
.discovery-inner p {
  color: var(--warm-gray);
  font-size: 18px; line-height: 1.8;
  margin-bottom: 10px;
}
.discovery-link {
  display: inline-block;
  margin-top: 20px;
  color: var(--terracotta);
  font-weight: 600;
  font-size: 14px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  border-bottom: 1px solid var(--terracotta);
  padding-bottom: 2px;
  transition: color 0.2s, border-color 0.2s;
}
.discovery-link:hover { color: var(--terracotta-deep); border-color: var(--terracotta-deep); }

/* ─── FOR WHO ─── */
.for-who {
  padding: 120px 0;
}

.section-eyebrow {
  font-family: var(--mono);
  font-size: 14px;
  letter-spacing: 0.10em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 20px;
}

.section-title {
  font-family: var(--display);
  font-size: clamp(32px, 5vw, 48px);
  font-weight: 400;
  letter-spacing: -0.01em;
  margin-bottom: 60px;
  line-height: 1.2;
}

.section-title em { color: var(--terracotta); font-style: italic; }

.situations-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2px;
  background: rgba(232,223,210,0.06);
}

.situation {
  padding: 36px 32px;
  background: var(--midnight);
  position: relative;
  overflow: hidden;
  transition: background 0.3s ease;
  cursor: default;
}

.situation::before {
  content: "";
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: var(--terracotta);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.4s cubic-bezier(0.22,1,0.36,1);
}

.situation:hover { background: rgba(58,40,86,0.6); }
.situation:hover::before { transform: scaleX(1); }

.situation-number {
  font-family: var(--display);
  font-size: 48px;
  font-weight: 300;
  line-height: 1;
  color: var(--cream);
  margin-bottom: 20px;
  transition: color 0.3s;
}
.situation:hover .situation-number { color: var(--cream); }

.situation h3 {
  font-family: var(--body);
  font-size: 15px;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--cream);
  margin-bottom: 12px;
}

.situation p {
  font-size: 16px;
  color: var(--warm-gray);
  line-height: 1.8;
}

/* ─── RPT DIMENSIONS ─── */
.dimensions {
  padding: 120px 0;
  position: relative;
  overflow: hidden;
}

.dimensions::before {
  content: "";
  position: absolute;
  top: 50%; left: -200px; transform: translateY(-50%);
  width: 600px; height: 600px;
  background: radial-gradient(ellipse, rgba(196,120,154,0.07) 0%, transparent 70%);
  pointer-events: none;
}

.dimensions-header {
  max-width: 760px;
  margin: 0 auto 80px;
}

.dimensions-header h2 {
  font-family: var(--display);
  font-size: clamp(32px, 5vw, 48px);
  font-weight: 400;
  line-height: 1.2;
  letter-spacing: -0.01em;
  margin-bottom: 24px;
}

.dimensions-header p {
  font-size: 18px;
  color: var(--warm-gray);
  line-height: 1.85;
  margin-bottom: 16px;
}

.dimensions-header .lead {
  font-family: var(--display);
  font-size: 24px;
  color: var(--cream);
  font-style: italic;
  font-weight: 400;
}

.pillars-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1px;
  background: rgba(232,223,210,0.06);
  margin-top: 16px;
}

.pillar {
  padding: 56px 40px;
  background: rgba(28,16,48,0.95);
  position: relative;
  overflow: hidden;
  transition: background 0.4s ease;
}

.pillar:hover { background: rgba(46,31,71,0.95); }

.pillar-accent {
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 3px;
}
.pillar:nth-child(1) .pillar-accent { background: var(--terracotta); }
.pillar:nth-child(2) .pillar-accent { background: #6AACBA; }
.pillar:nth-child(2) .pillar-questions li::before { color: #6AACBA; }
.pillar:nth-child(2) .pillar-benefit { background: rgba(106,172,186,0.08); border-color: rgba(106,172,186,0.18); }
.pillar:nth-child(3) .pillar-accent { background: #D4B483; }
.pillar:nth-child(3) .pillar-questions li::before { color: #D4B483; }
.pillar:nth-child(3) .pillar-benefit { background: rgba(212,180,131,0.08); border-color: rgba(212,180,131,0.18); }

.pillar-letter {
  font-family: var(--display);
  font-size: 160px;
  font-weight: 300;
  line-height: 0.8;
  margin-bottom: 28px;
  opacity: 0.12;
  transition: opacity 0.3s;
  user-select: none;
}
.pillar:nth-child(1) .pillar-letter { color: var(--terracotta); }
.pillar:nth-child(2) .pillar-letter { color: #7EC8D8; }
.pillar:nth-child(2) .pillar-title { color: #A8D8E4; }
.pillar:nth-child(3) .pillar-letter { color: #D4B483; }
.pillar:nth-child(3) .pillar-title { color: #DFC99A; }
.pillar:hover .pillar-letter { opacity: 0.2; }

.pillar-title {
  font-family: var(--display);
  font-size: 32px;
  font-weight: 500;
  letter-spacing: 0.04em;
  margin-bottom: 8px;
  color: var(--cream);
}

.pillar-subtitle {
  font-family: var(--mono);
  font-size: 12px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--warm-gray-light);
  margin-bottom: 28px;
}

.pillar-intro {
  font-size: 17px;
  color: var(--warm-gray-light);
  line-height: 1.9;
  margin-bottom: 28px;
}

.pillar-questions {
  list-style: none;
  margin-bottom: 28px;
  border-left: 1px solid rgba(232,223,210,0.1);
  padding-left: 16px;
}

.pillar-questions li {
  margin-bottom: 14px;
  font-size: 16px;
  line-height: 1.6;
  color: var(--warm-gray-light);
  position: relative;
}

.pillar-questions li::before {
  content: "→";
  position: absolute;
  left: -24px;
  font-size: 11px;
  color: var(--terracotta);
  opacity: 0.6;
}

.pillar-benefit {
  padding: 22px;
  background: rgba(232,223,210,0.07);
  border: 1px solid rgba(232,223,210,0.14);
  font-size: 17px;
  font-weight: 600;
  color: var(--cream);
  letter-spacing: 0.02em;
  line-height: 1.6;
}

.pillar-benefit em {
  display: block;
  margin-top: 8px;
  font-style: italic;
  font-weight: 400;
  color: var(--cream);
  font-family: var(--body);
  font-size: 16px;
  opacity: 0.9;
  font-style: italic;
}

/* ─── AVANT / APRÈS ─── */
.before-after {
  padding: 120px 0;
  background: rgba(58,40,86,0.15);
  border-top: 1px solid rgba(232,223,210,0.06);
  border-bottom: 1px solid rgba(232,223,210,0.06);
}

.before-after-header {
  max-width: 600px;
  margin: 0 auto 64px;
  text-align: center;
}

.ba-grid {
  display: grid;
  gap: 2px;
  background: rgba(232,223,210,0.06);
}

.ba-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2px;
  background: rgba(232,223,210,0.06);
  transition: background 0.3s;
}
.ba-row:hover { background: rgba(196,120,154,0.06); }

.ba-cell {
  padding: 32px 36px;
  background: var(--midnight);
}

.ba-cell.before {
  background: rgba(28,16,48,0.98);
  border-left: 2px solid rgba(232,223,210,0.08);
}

.ba-cell.after {
  background: rgba(46,31,71,0.5);
  border-left: 2px solid var(--terracotta);
}

.ba-label {
  font-family: var(--mono);
  font-size: 12px;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  margin-bottom: 12px;
}

.ba-cell.before .ba-label { color: var(--warm-gray); }
.ba-cell.after .ba-label { color: var(--terracotta); }

.ba-problem {
  font-size: 18px;
  font-weight: 600;
  color: var(--cream);
  margin-bottom: 12px;
}

.ba-solution {
  font-size: 16px;
  color: var(--warm-gray);
  line-height: 1.75;
}

.ba-solution span {
  display: block;
  margin-bottom: 6px;
  padding-left: 16px;
  position: relative;
}

.ba-solution span::before {
  content: "✓";
  position: absolute; left: 0;
  color: var(--terracotta);
  font-size: 13px;
}

.ba-solution span.key {
  color: var(--cream);
  font-weight: 500;
}

/* ─── WHO IS INÈS ─── */
.who-is {
  padding: 0;
  overflow: hidden;
}

.who-is-grid { display: none; }

.who-is-text h2 {
  font-family: var(--display);
  font-size: clamp(28px, 4vw, 40px);
  font-weight: 400;
  margin-bottom: 32px;
  letter-spacing: -0.01em;
  line-height: 1.25;
}

.who-is-text p {
  font-size: 18px;
  color: var(--warm-gray);
  line-height: 1.85;
  margin-bottom: 20px;
}

.who-is-text p strong { color: var(--cream); font-weight: 600; }

.conviction-block {
  margin-top: 32px;
  padding: 28px 32px;
  border-left: 3px solid var(--terracotta);
  background: rgba(196,120,154,0.06);
  font-family: var(--body);
  font-size: 19px;
  font-weight: 400;
  font-style: italic;
  color: var(--cream);
  line-height: 1.7;
}

.who-is-sidebar {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.stat-card {
  padding: 28px 24px;
  background: rgba(58,40,86,0.4);
  border: 1px solid rgba(232,223,210,0.08);
  position: relative;
  overflow: hidden;
  transition: border-color 0.3s;
}
.stat-card:hover { border-color: rgba(196,120,154,0.25); }

.stat-card::before {
  content: "";
  position: absolute; top: 0; left: 0;
  width: 3px; height: 100%;
  background: var(--terracotta);
  opacity: 0.4;
}

.stat-number {
  font-family: var(--display);
  font-size: 52px;
  font-weight: 400;
  color: var(--terracotta);
  line-height: 1;
  margin-bottom: 6px;
}

.stat-label {
  font-size: 16px;
  color: var(--warm-gray);
  font-weight: 500;
  letter-spacing: 0.04em;
}

.credentials {
  margin-top: 24px;
  padding: 24px;
  background: rgba(28,16,48,0.8);
  border: 1px solid rgba(232,223,210,0.06);
}

.credentials-title {
  font-family: var(--mono);
  font-size: 13px;
  letter-spacing: 0.10em;
  text-transform: uppercase;
  color: var(--warm-gray);
  margin-bottom: 16px;
}

.cert-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 10px 16px;
  background: rgba(196,120,154,0.1);
  border: 1px solid rgba(196,120,154,0.2);
  font-family: var(--mono);
  font-size: 14px;
  color: var(--terracotta-pale);
  margin: 4px 4px 0 0;
}

/* ─── OFFER ─── */
.offer {
  padding: 120px 0;
  background: linear-gradient(135deg, rgba(58,40,86,0.4) 0%, rgba(28,16,48,0.8) 100%);
  border-top: 1px solid rgba(232,223,210,0.06);
}

.offer-card {
  max-width: 720px;
  margin: 0 auto;
  padding: 64px 56px;
  background: rgba(46,31,71,0.7);
  border: 1px solid rgba(232,223,210,0.12);
  position: relative;
  overflow: hidden;
}

.offer-card::before {
  content: "";
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 3px;
  background: linear-gradient(90deg, var(--terracotta), var(--teal));
}

.offer-card::after {
  content: "R.P.T.";
  position: absolute;
  bottom: -20px; right: -10px;
  font-family: var(--display);
  font-size: 180px;
  font-weight: 300;
  color: rgba(232,223,210,0.025);
  letter-spacing: -0.05em;
  line-height: 1;
  user-select: none;
}

.offer-title {
  font-family: var(--display);
  font-size: 40px;
  font-weight: 400;
  letter-spacing: -0.01em;
  margin-bottom: 8px;
  color: var(--cream);
}

.offer-badge {
  display: inline-block;
  padding: 6px 16px;
  background: rgba(196,120,154,0.12);
  border: 1px solid rgba(196,120,154,0.25);
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--terracotta-pale);
  margin-bottom: 32px;
}

.offer-desc {
  font-size: 18px;
  color: var(--warm-gray);
  line-height: 1.85;
  margin-bottom: 8px;
}

.offer-desc strong { color: var(--cream); }

.offer-list {
  list-style: none;
  margin: 28px 0 36px;
}

.offer-list li {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 16px 0;
  border-bottom: 1px solid rgba(232,223,210,0.06);
  font-size: 17px;
  color: var(--warm-gray);
  line-height: 1.6;
}

.offer-list li:last-child { border-bottom: none; }

.offer-list li::before {
  content: "✓";
  flex-shrink: 0;
  width: 20px; height: 20px;
  display: flex; align-items: center; justify-content: center;
  background: rgba(196,120,154,0.15);
  color: var(--terracotta);
  font-size: 12px;
  font-weight: 700;
  margin-top: 2px;
}

.offer-decision {
  padding: 24px;
  background: rgba(232,223,210,0.04);
  border: 1px solid rgba(232,223,210,0.08);
  margin-bottom: 32px;
  font-size: 17px;
  color: var(--warm-gray);
  line-height: 1.8;
}

.offer-decision strong { color: var(--cream); display: block; margin-bottom: 8px; }

/* ─── FOOTER CTA ─── */
.footer-cta {
  padding: 100px 0;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.footer-cta::before {
  content: "";
  position: absolute;
  top: 50%; left: 50%; transform: translate(-50%,-50%);
  width: 600px; height: 600px;
  background: radial-gradient(ellipse, rgba(196,120,154,0.08) 0%, transparent 65%);
  pointer-events: none;
}

.footer-cta h2 {
  font-family: var(--display);
  font-size: clamp(32px, 5vw, 52px);
  font-weight: 400;
  letter-spacing: -0.02em;
  line-height: 1.2;
  margin-bottom: 20px;
  position: relative; z-index: 1;
}

.footer-cta p {
  font-size: 18px;
  color: var(--warm-gray);
  max-width: 520px;
  margin: 0 auto 40px;
  line-height: 1.8;
  position: relative; z-index: 1;
}

/* ─── FOOTER ─── */
.footer {
  padding: 40px 0;
  border-top: 1px solid rgba(232,223,210,0.06);
  background: rgba(28,16,48,0.8);
}

.footer-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 16px;
}

.footer-copy {
  font-size: 16px;
  color: var(--warm-gray);
  line-height: 1.6;
}

.footer-credit {
  font-size: 11px;
  color: rgba(176,165,192,0.5);
  font-family: var(--mono);
  letter-spacing: 0.08em;
  text-align: right;
}

.footer-credit span {
  color: rgba(196,120,154,0.5);
}

/* ─── RESPONSIVE ─── */
@media (max-width: 900px) {
  .pillars-grid { grid-template-columns: 1fr; }
  .who-is-grid  { grid-template-columns: 1fr; gap: 40px; }
  .ba-row       { grid-template-columns: 1fr; }
  .container    { padding: 0 24px; }
  .offer-card   { padding: 40px 28px; }
}

@media (max-width: 600px) {
  .situations-grid { grid-template-columns: repeat(2, 1fr); }
  .hero-cta-group  { flex-direction: column; align-items: center; }
  .nav-tag         { display: none; }
}

/* ─── SECTION À PROPOS — REDESIGN ÉDITORIAL ─── */
.who-is-photo { display: none; } /* masqué — remplacé par le nouveau layout */

/* ─── FOOTER LINKS ─── */
.footer-links {
  display: flex;
  align-items: center;
  gap: 24px;
  flex-wrap: wrap;
  justify-content: flex-end;
}

.footer-link {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  font-size: 16px;
  color: var(--warm-gray);
  transition: color 0.2s;
  letter-spacing: 0.03em;
}

.footer-link:hover { color: var(--cream); }

.footer-link-cta {
  padding: 8px 16px;
  background: rgba(196,120,154,0.12);
  border: 1px solid rgba(196,120,154,0.25);
  color: var(--terracotta-pale);
}

.footer-link-cta:hover {
  background: rgba(196,120,154,0.2);
  color: var(--cream);
}




/* ═══════════════════════════════════════════════
   RESPONSIVE — MOBILE FIRST (max-width breakpoints)
   ═══════════════════════════════════════════════ */

/* ── Tablet (≤ 1024px) ── */
@media (max-width: 1024px) {
  .container { padding: 0 32px; }
  .nav-inner { padding: 18px 32px; }

  .pillars-grid { grid-template-columns: 1fr; gap: 2px; }
  .pillar { padding: 44px 36px; }

  .who-is-grid {
    grid-template-columns: 1fr 300px;
    gap: 48px;
  }

  .who-is-photo { display: none; }

  .offer-card { padding: 52px 44px; }
}

/* ── Mobile Large (≤ 768px) ── */
@media (max-width: 768px) {
  body { font-size: 17px; }

  .container { padding: 0 20px; }
  .nav-inner { padding: 16px 20px; }
  .nav-tag { display: none; }
  .logo { font-size: 20px; }

  /* Hero */
  .hero { padding: 120px 0 80px; min-height: auto; }
  .hero h1 { font-size: clamp(34px, 10vw, 52px); margin-bottom: 24px; }
  .hero-label { font-size: 12px; padding: 7px 16px; margin-bottom: 28px; }
  .hero-sub { font-size: 18px; }
  .hero-promise { font-size: 19px; }
  .hero-cta-group { flex-direction: column; align-items: stretch; gap: 12px; }
  .btn-primary, .btn-ghost { width: 100%; justify-content: center; padding: 18px 24px; font-size: 15px; }
  .hero-scroll { display: none; }

  /* Marquee */
  .marquee-item { font-size: 12px; }

  /* Discovery */
  .discovery { padding: 60px 0; }
  .discovery-inner { padding: 40px 28px; }
  .discovery-inner h2 { font-size: 28px; }
  .discovery-inner p { font-size: 16px; }

  /* For who */
  .for-who { padding: 80px 0; }
  .section-title { font-size: clamp(28px, 7vw, 38px); margin-bottom: 40px; }
  .section-eyebrow { font-size: 12px; }
  .situations-grid { grid-template-columns: repeat(2, 1fr); }
}

@media (max-width: 500px) {
  .situations-grid { grid-template-columns: 1fr !important; }
  .situation { padding: 28px 24px; }
  .situation-number { font-size: 40px; margin-bottom: 14px; }
  .situation h3 { font-size: 15px; }
  .situation p { font-size: 15px; }


  /* Dimensions */
  .dimensions { padding: 80px 0; }
  .dimensions-header { margin-bottom: 48px; }
  .dimensions-header h2 { font-size: clamp(28px, 7vw, 38px); }
  .dimensions-header p { font-size: 16px; }
  .dimensions-header .lead { font-size: 20px; }
  .pillars-grid { grid-template-columns: 1fr; }
  .pillar { padding: 36px 24px; }
  .pillar-letter { font-size: 110px; }
  .pillar-title { font-size: 26px; }
  .pillar-intro { font-size: 15px; }
  .pillar-questions li { font-size: 14px; }
  .pillar-benefit { font-size: 14px; }

  /* Before/After */
  .before-after { padding: 80px 0; }
  .ba-row { grid-template-columns: 1fr; }
  .ba-cell { padding: 24px 20px; }
  .ba-cell.before { border-left: none; border-top: 2px solid rgba(232,223,210,0.08); }
  .ba-cell.after { border-left: 2px solid var(--terracotta); }
  .ba-problem { font-size: 16px; }
  .ba-solution { font-size: 15px; }
  .ba-label { font-size: 11px; }

  /* Who is */
  .who-is { padding: 80px 0; }
  .who-is-photo { display: none; }
  .who-is-grid { grid-template-columns: 1fr; gap: 40px; }
  .who-is-text h2 { font-size: clamp(26px, 7vw, 36px); }
  .who-is-text p { font-size: 16px; }
  .conviction-block { font-size: 19px; padding: 24px; }
  .who-is-sidebar {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
  }
  .credentials { grid-column: 1 / -1; }
  .stat-number { font-size: 40px; }
  .stat-label { font-size: 14px; }

  /* Offer */
  .offer { padding: 80px 0; }
  .offer-card { padding: 36px 24px; }
  .offer-title { font-size: 32px; }
  .offer-badge { font-size: 11px; }
  .offer-desc { font-size: 16px; }
  .offer-list li { font-size: 15px; padding: 14px 0; }
  .offer-decision { font-size: 15px; }
  .offer-card::after { font-size: 120px; bottom: -10px; right: -5px; }

  /* Footer CTA */
  .footer-cta { padding: 80px 0; }
  .footer-cta h2 { font-size: clamp(28px, 7vw, 40px); }
  .footer-cta p { font-size: 17px; }

  /* Footer */
  .footer { padding: 36px 0; }
  .footer-inner { flex-direction: column; align-items: flex-start; gap: 20px; }
  .footer-copy { font-size: 14px; }
  .footer-links { gap: 12px; flex-wrap: wrap; }
  .footer-link { font-size: 14px; }
}

/* ── Mobile Small (≤ 480px) ── */
@media (max-width: 480px) {
  body { font-size: 16px; }
  .container { padding: 0 16px; }
  .nav-inner { padding: 14px 16px; }

  .hero { padding: 100px 0 60px; }
  .hero h1 { font-size: clamp(30px, 9vw, 44px); }
  .hero-label { font-size: 11px; padding: 6px 14px; }
  .hero-sub { font-size: 17px; }
  .hero-promise { font-size: 17px; }

  .section-title { font-size: clamp(26px, 8vw, 34px); }
  .discovery-inner h2 { font-size: 24px; }
  .dimensions-header h2 { font-size: clamp(24px, 8vw, 32px); }

  .who-is-sidebar { grid-template-columns: 1fr; }
  .stat-number { font-size: 38px; }

  .offer-card { padding: 28px 18px; }
  .offer-title { font-size: 28px; }

  .footer-cta h2 { font-size: clamp(24px, 8vw, 34px); }

  .pillar-letter { font-size: 90px; }
  .ba-cell { padding: 20px 16px; }

  .btn-primary, .btn-ghost { font-size: 15px; padding: 16px 20px; }
}

/* ── Very Small (≤ 360px) ── */
@media (max-width: 360px) {
  .hero h1 { font-size: 28px; }
  .section-title { font-size: 24px; }
  .offer-title { font-size: 24px; }
  .footer-cta h2 { font-size: 24px; }
  .conviction-block { font-size: 17px; }
}


/* ════════════════════════════════════════
   SECTION À PROPOS — ÉDITORIAL REDESIGN
   ════════════════════════════════════════ */

.about-wrapper {
  display: grid;
  grid-template-columns: 480px 1fr;
  min-height: 90vh;
}

/* ── Photo column ── */
.about-photo-col {
  position: relative;
  background: var(--deep-violet);
  display: flex;
  flex-direction: column;
}

.about-photo-inner {
  position: relative;
  flex: 1;
  overflow: hidden;
}

.about-photo-inner img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center top;
  display: block;
  filter: saturate(0.85) contrast(1.08);
  mix-blend-mode: normal;
}

/* Gradient overlay sur la photo */
.about-photo-inner::after {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(28,16,48,0.05) 0%,
    rgba(28,16,48,0.3) 70%,
    rgba(28,16,48,0.85) 100%
  );
}

/* Tag 17 ans flottant sur la photo */


/* Ligne décorative verticale */
.about-photo-line {
  position: absolute;
  top: 40px; right: 0;
  width: 3px;
  height: 80px;
  background: var(--terracotta);
}

/* Stats sous la photo */
.about-stats {
  display: flex;
  flex-direction: column;
  gap: 0;
  border-top: 1px solid rgba(232,223,210,0.08);
}

.about-stat {
  padding: 20px 32px;
  border-bottom: 1px solid rgba(232,223,210,0.06);
  display: flex;
  align-items: center;
  gap: 20px;
  transition: background 0.3s;
}

.about-stat:hover {
  background: rgba(196,120,154,0.06);
}

.about-stat-num {
  font-family: var(--display);
  font-size: 36px;
  font-weight: 400;
  color: var(--terracotta);
  line-height: 1;
  min-width: 60px;
}

.about-stat-label {
  font-size: 13px;
  color: var(--warm-gray);
  line-height: 1.5;
  letter-spacing: 0.02em;
}

/* ── Content column ── */
.about-content-col {
  background: var(--midnight);
  padding: 80px 64px 80px 72px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;
  border-left: 1px solid rgba(232,223,210,0.06);
}

/* Filigrane décoratif en fond */
.about-content-col::before {
  content: "À PROPOS";
  position: absolute;
  top: 40px; right: -20px;
  font-family: var(--display);
  font-size: 120px;
  font-weight: 300;
  color: rgba(232,223,210,0.025);
  letter-spacing: -0.04em;
  line-height: 1;
  user-select: none;
  writing-mode: vertical-rl;
  text-orientation: mixed;
}

.about-eyebrow {
  font-family: var(--mono);
  font-size: 12px;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 28px;
}

.about-title {
  font-family: var(--display);
  font-size: clamp(36px, 4.5vw, 58px);
  font-weight: 400;
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--cream);
  margin-bottom: 36px;
}

.about-title em {
  color: var(--terracotta);
  font-style: italic;
}

.about-divider-h {
  width: 48px;
  height: 2px;
  background: var(--terracotta);
  margin-bottom: 36px;
  opacity: 0.7;
}

.about-body {
  margin-bottom: 36px;
}

.about-body p {
  font-size: 16px;
  color: var(--warm-gray);
  line-height: 1.85;
  margin-bottom: 18px;
}

.about-body p strong {
  color: var(--cream);
  font-weight: 500;
}

.about-quote {
  margin: 0 0 40px;
  padding: 24px 28px;
  border-left: 3px solid var(--terracotta);
  background: rgba(196,120,154,0.05);
  font-family: var(--display);
  font-size: 19px;
  font-style: italic;
  color: var(--cream);
  line-height: 1.65;
}

.about-certs {
  display: flex;
  align-items: center;
  gap: 16px;
  flex-wrap: wrap;
  padding-top: 28px;
  border-top: 1px solid rgba(232,223,210,0.07);
}

.about-cert-label {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--warm-gray);
}

.about-cert-badges {
  display: flex;
  align-items: center;
  gap: 10px;
  flex-wrap: wrap;
}

.about-cert {
  font-family: var(--mono);
  font-size: 13px;
  color: var(--terracotta-pale);
  letter-spacing: 0.08em;
}

.about-cert-dot {
  color: rgba(196,120,154,0.4);
  font-size: 18px;
}

/* ── RESPONSIVE ABOUT ── */
@media (max-width: 1024px) {
  .about-wrapper {
    grid-template-columns: 380px 1fr;
  }
  .about-content-col {
    padding: 60px 48px;
  }
}

@media (max-width: 768px) {
  .about-wrapper {
    grid-template-columns: 1fr;
    min-height: auto;
  }

  .about-photo-col {
    height: 500px;
    flex-direction: row;
    flex-wrap: wrap;
  }

  .about-photo-inner {
    width: 100%;
    height: 340px;
    flex: none;
  }

  .about-stats {
    flex-direction: row;
    width: 100%;
    border-top: none;
    background: rgba(28,16,48,0.95);
  }

  .about-stat {
    flex: 1;
    flex-direction: column;
    align-items: flex-start;
    gap: 4px;
    padding: 16px 16px;
    border-bottom: none;
    border-right: 1px solid rgba(232,223,210,0.06);
  }

  .about-stat:last-child { border-right: none; }

  .about-stat-num { font-size: 28px; min-width: auto; }
  .about-stat-label { font-size: 11px; }



  .about-content-col {
    padding: 48px 24px;
    border-left: none;
    border-top: 1px solid rgba(232,223,210,0.06);
  }

  .about-content-col::before { display: none; }
  .about-title { font-size: 36px; }
  .about-quote { font-size: 17px; padding: 20px; }
}

@media (max-width: 480px) {
  .about-photo-inner { height: 280px; }
  .about-photo-col { height: auto; }
  .about-stats { flex-direction: column; }
  .about-stat { flex-direction: row; border-right: none; border-bottom: 1px solid rgba(232,223,210,0.06); }
  .about-stat-num { min-width: 50px; font-size: 26px; }
  .about-title { font-size: 30px; }
}


/* ─── WHATSAPP FLOTTANT ─── */
.whatsapp-btn {
  position: fixed;
  bottom: 32px;
  right: 32px;
  z-index: 9999;
  display: flex;
  align-items: center;
  gap: 12px;
  background: #25D366;
  color: white;
  text-decoration: none;
  padding: 14px 22px 14px 16px;
  border-radius: 50px;
  box-shadow: 0 8px 32px rgba(37, 211, 102, 0.35), 0 2px 8px rgba(0,0,0,0.25);
  transition: all 0.35s cubic-bezier(0.22, 1, 0.36, 1);
  overflow: hidden;
  max-width: 240px;
}

.whatsapp-btn:hover {
  background: #1ebe5d;
  transform: translateY(-3px);
  box-shadow: 0 14px 40px rgba(37, 211, 102, 0.45), 0 4px 12px rgba(0,0,0,0.3);
  max-width: 260px;
}

.whatsapp-icon {
  width: 36px;
  height: 36px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.whatsapp-label {
  font-family: var(--body);
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 0.02em;
  white-space: nowrap;
}

/* Pulse animation */
.whatsapp-pulse {
  position: absolute;
  inset: 0;
  border-radius: 50px;
  border: 2px solid rgba(37, 211, 102, 0.6);
  animation: wa-pulse 2.5s ease-out infinite;
  pointer-events: none;
}

@keyframes wa-pulse {
  0%   { transform: scale(1); opacity: 0.8; }
  70%  { transform: scale(1.12); opacity: 0; }
  100% { transform: scale(1.12); opacity: 0; }
}

/* Mobile — icône seule, label masqué */
@media (max-width: 600px) {
  .whatsapp-btn {
    bottom: 20px;
    left: 50%;
    right: auto;
    transform: translateX(-50%);
    padding: 14px 28px;
    border-radius: 50px;
    max-width: 220px;
    width: auto;
    height: auto;
    justify-content: center;
    align-items: center;
  }
  .whatsapp-label { display: block; font-size: 14px; }
  .whatsapp-btn:hover { max-width: 240px; transform: translateX(-50%) translateY(-3px); }
  .whatsapp-icon { width: 28px; height: 28px; }
  .whatsapp-icon svg { width: 24px; height: 24px; }
}


/* ===== V7 MODS — additional styling ===== */
.for-who-main-title {
  font-size: clamp(48px, 6vw, 84px) !important;
  text-align: center;
  margin-bottom: 24px;
}
.for-who-subtitle {
  text-align: center;
  font-family: var(--display);
  font-size: clamp(20px, 2.4vw, 28px);
  color: var(--pearl);
  margin-bottom: 64px;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
  font-weight: 400;
}

.situation-bridge {
  background: linear-gradient(135deg, rgba(196, 120, 154, 0.18), rgba(196, 120, 154, 0.06)) !important;
  border: 1px solid rgba(196, 120, 154, 0.4) !important;
  position: relative;
}
.situation-bridge::before {
  content: "→";
  position: absolute;
  top: -14px;
  right: 24px;
  font-family: var(--display);
  font-size: 32px;
  color: var(--terracotta);
  background: var(--midnight);
  padding: 0 12px;
  line-height: 1;
}
.situation-bridge h3 {
  color: var(--terracotta) !important;
}

.dimensions-main-title {
  font-size: clamp(48px, 6vw, 84px) !important;
  margin-bottom: 24px;
}
.dimensions-subtitle {
  font-family: var(--display);
  font-size: clamp(24px, 5vw, 70px);
  color: var(--pearl);
  margin-bottom: 32px;
  max-width: 1100px;
  font-weight: 400;
  line-height: 1.2;
  letter-spacing: -0.01em;
}

.ba-main-title {
  font-size: clamp(36px, 4.5vw, 64px) !important;
  text-align: center;
  margin-bottom: 16px;
  line-height: 1.15;
}
.ba-arrow {
  color: var(--terracotta);
  font-style: normal;
  font-weight: 400;
  margin: 0 12px;
}
.ba-subtitle {
  text-align: center;
  font-family: var(--display);
  font-size: clamp(18px, 2vw, 24px);
  color: var(--pearl);
  margin-bottom: 64px;
  font-weight: 400;
  font-style: normal;
}
.ba-cell .ba-problem,
.ba-cell .ba-solution span {
  font-family: var(--body) !important;
  font-style: normal !important;
  font-weight: 400 !important;
  font-size: 16px !important;
  line-height: 1.55 !important;
  color: var(--cream) !important;
}
.ba-cell .ba-solution span.key {
  font-weight: 500 !important;
}

.about-eyebrow-large {
  font-size: clamp(48px, 6vw, 84px) !important;
  font-family: var(--display) !important;
  color: var(--cream) !important;
  text-transform: none !important;
  letter-spacing: -0.01em !important;
  margin-bottom: 16px !important;
  font-weight: 500 !important;
}
.about-job-title {
  font-family: var(--display);
  font-style: italic;
  font-size: clamp(18px, 2vw, 24px);
  color: var(--terracotta);
  margin-bottom: 32px;
  font-weight: 400;
  line-height: 1.4;
}
.about-frameworks {
  font-style: normal;
  font-weight: 600;
  color: var(--terracotta);
  font-family: var(--display);
}
.about-link {
  color: inherit;
  text-decoration: underline;
  text-decoration-thickness: 1px;
  text-underline-offset: 3px;
  transition: color 0.2s;
}
.about-link:hover {
  color: var(--terracotta);
}

.marquee-bridge {
  background: linear-gradient(90deg, transparent, rgba(196, 120, 154, 0.12), transparent) !important;
  padding: 18px 0 !important;
  border-top: 1px solid rgba(196, 120, 154, 0.2);
  border-bottom: 1px solid rgba(196, 120, 154, 0.2);
}
.bridge-item {
  font-family: var(--display) !important;
  font-style: italic;
  font-size: 18px !important;
  letter-spacing: 0.02em !important;
  color: var(--pearl) !important;
}

.newsletter-section {
  padding: 100px 0 80px;
  background: var(--midnight);
  border-top: 1px solid rgba(250, 247, 242, 0.06);
}
.newsletter-card {
  max-width: 820px;
  margin: 0 auto;
  text-align: center;
  padding: 48px 32px;
  background: linear-gradient(135deg, rgba(196, 120, 154, 0.10), rgba(196, 120, 154, 0.02));
  border: 1px solid rgba(196, 120, 154, 0.25);
  border-radius: 4px;
  position: relative;
}
.newsletter-card::before {
  content: "";
  position: absolute;
  inset: 12px;
  border: 1px solid rgba(250, 247, 242, 0.05);
  pointer-events: none;
}
.newsletter-eyebrow {
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--terracotta);
  margin-bottom: 24px;
  position: relative;
}
.newsletter-title {
  font-family: var(--display);
  font-size: clamp(32px, 4vw, 52px);
  font-weight: 500;
  line-height: 1.15;
  color: var(--cream);
  margin-bottom: 20px;
  letter-spacing: -0.005em;
  position: relative;
}
.newsletter-title em {
  color: var(--terracotta);
  font-style: italic;
}
.newsletter-desc {
  font-family: var(--display);
  font-size: clamp(16px, 1.6vw, 19px);
  line-height: 1.55;
  color: var(--pearl);
  max-width: 640px;
  margin: 0 auto 36px;
  font-style: italic;
  font-weight: 400;
  position: relative;
}
.newsletter-cta {
  display: inline-flex;
  align-items: center;
  position: relative;
}

.footer-inner-split {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 24px;
  padding-bottom: 24px;
  border-bottom: 1px solid rgba(250, 247, 242, 0.08);
}
.footer-links-left,
.footer-links-right {
  display: flex;
  gap: 24px;
  flex-wrap: wrap;
}
.footer-copy-bottom {
  text-align: center;
  padding-top: 24px;
  font-family: var(--mono);
  font-size: 11px;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  color: var(--warm-gray);
}
@media (max-width: 700px) {
  .footer-inner-split {
    flex-direction: column;
    align-items: flex-start;
    text-align: left;
  }
  .footer-links-right {
    align-self: flex-start;
  }
}
/* ===== END V7 MODS ===== */

/* ===== À PROPOS — Photo title + R.P.T. definitions ===== */
.about-photo-title {
  margin-top: 28px;
  padding: 18px 0 4px;
  text-align: center;
  font-family: var(--display);
  position: relative;
}
.about-photo-title-prefix {
  display: block;
  font-style: italic;
  font-weight: 400;
  color: var(--pearl);
  font-size: clamp(14px, 1.4vw, 17px);
  letter-spacing: 0.04em;
  margin-bottom: 8px;
  opacity: 0.85;
}
.about-rpt-letters {
  display: inline-flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: baseline;
  gap: 8px;
  font-family: var(--display);
  font-weight: 500;
  font-size: clamp(18px, 2vw, 24px);
  letter-spacing: -0.005em;
  line-height: 1.2;
}
.about-rpt-letters .rpt-r,
.about-rpt-letters .rpt-p,
.about-rpt-letters .rpt-t {
  position: relative;
  color: var(--cream);
  padding: 0 2px;
}
.about-rpt-letters .rpt-r::after,
.about-rpt-letters .rpt-p::after,
.about-rpt-letters .rpt-t::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  bottom: -3px;
  height: 2px;
  border-radius: 2px;
}
.about-rpt-letters .rpt-r::after { background: var(--terracotta); }
.about-rpt-letters .rpt-p::after { background: #4B7F8C; }
.about-rpt-letters .rpt-t::after { background: #6B8068; }
.about-rpt-letters .rpt-sep {
  color: var(--terracotta);
  font-style: normal;
  font-weight: 400;
  opacity: 0.75;
}

/* Bio paragraphs — 12pt larger, more readable */
.about-body p {
  font-size: clamp(18px, 1.7vw, 22px) !important;
  line-height: 1.65 !important;
}

/* R.P.T. definitions list — all normal (no italic anywhere) */
.rpt-definitions {
  margin: 36px 0 8px;
  padding: 0;
  display: flex;
  flex-direction: column;
  gap: 22px;
  position: relative;
}
.rpt-definitions::before {
  content: "";
  position: absolute;
  left: 0;
  top: 6px;
  bottom: 6px;
  width: 2px;
  background: linear-gradient(to bottom, var(--terracotta) 0%, #4B7F8C 50%, #6B8068 100%);
  opacity: 0.55;
}
.rpt-def {
  padding-left: 24px;
  position: relative;
}
.rpt-def dt {
  font-family: var(--display);
  font-weight: 500;
  font-style: normal !important;
  font-size: clamp(22px, 2.4vw, 28px);
  line-height: 1.1;
  margin-bottom: 6px;
  display: flex;
  align-items: baseline;
  gap: 2px;
}
.rpt-def .rpt-letter {
  font-size: 1.5em;
  font-weight: 600;
  font-style: normal !important;
}
.rpt-def .rpt-word {
  letter-spacing: 0.04em;
  font-size: 0.85em;
  color: var(--cream);
  font-style: normal !important;
  font-variant: normal !important;
  text-transform: none;
}
.rpt-def-r .rpt-letter { color: var(--terracotta); }
.rpt-def-p .rpt-letter { color: #4B7F8C; }
.rpt-def-t .rpt-letter { color: #6B8068; }
.rpt-def dd {
  margin: 0;
  font-family: var(--display);
  font-style: normal !important;
  font-weight: 400;
  font-size: clamp(18px, 1.8vw, 21px);
  line-height: 1.5;
  color: var(--pearl);
}

/* Title above certifications */
.about-cert-title {
  font-family: var(--display);
  font-style: normal;
  font-weight: 500;
  font-size: clamp(18px, 1.9vw, 22px);
  color: var(--cream);
  margin-bottom: 16px;
  letter-spacing: -0.005em;
  line-height: 1.3;
}

/* Bridge marquee — non italic, blanc nacré, Cormorant */
.bridge-item {
  font-family: var(--display) !important;
  font-style: normal !important;
  font-weight: 500 !important;
  font-size: 19px !important;
  letter-spacing: 0.01em !important;
  color: var(--cream) !important;
}

/* Newsletter title with inline LinkedIn icon + smaller decoding */
.newsletter-title {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 14px;
}
.newsletter-linkedin-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  color: var(--terracotta);
  flex-shrink: 0;
}
.newsletter-decoding {
  font-style: normal;
  font-weight: 500;
  font-size: 0.7em;
  color: var(--terracotta);
  letter-spacing: 0.005em;
}
.newsletter-desc {
  font-style: normal !important;
  font-weight: 400 !important;
  font-size: clamp(18px, 1.9vw, 22px) !important;
  line-height: 1.6 !important;
}

/* Footer CTA — remove gray radial glow that competes with button */
.footer-cta::before { display: none !important; }

/* Title above certifications */
.about-cert-title { font-style: normal; }

/* Section titles forced on single line */
.dimensions-main-title {
  white-space: nowrap;
  font-size: clamp(28px, 5.2vw, 72px) !important;
}

/* Avant/Après title — toujours sur deux lignes, design éditorial avec filet central */
.ba-main-title {
  white-space: normal;
  font-size: clamp(24px, 4vw, 52px) !important;
  line-height: 1.2;
  letter-spacing: -0.01em;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
}
.ba-main-title .ba-arrow {
  display: block;
  margin: 10px 0 !important;
  font-size: 0;
  line-height: 0;
  width: 64px;
  height: 1px;
  background: var(--terracotta);
  opacity: 0.55;
}
.ba-main-title .ba-rpt {
  color: var(--terracotta);
  font-weight: 500;
}

/* "R.P.T." en rose dans le titre Avant/Après */
.ba-rpt {
  color: var(--terracotta);
  font-weight: 500;
}

/* ===== TOUS LES GRANDS TITRES DE SECTION EN ROSE POUDRÉ ===== */
.for-who-main-title,
.dimensions-main-title,
.ba-main-title,
.about-eyebrow-large,
.offer-title {
  color: var(--terracotta) !important;
}
/* Les éléments enfants <em> de ces titres restent en accent contrasté (cream) */
.for-who-main-title em,
.dimensions-main-title em,
.offer-title em {
  color: var(--cream) !important;
}
/* "Decoding the System" reste rose dans le titre newsletter (pas de surcharge) */
.newsletter-decoding {
  color: var(--terracotta) !important;
}

/* Hero h1 em — "clarté stratégique" en typo normale (pas d'italique) */
.hero h1 em {
  font-style: normal !important;
}

/* Footer link icons — couleurs propres aux marques */
.footer-links-left .footer-link:nth-child(1) svg {
  color: #0A66C2 !important; /* LinkedIn blue */
}
.footer-links-left .footer-link:nth-child(2) svg {
  color: #EA4335 !important; /* Email red (Gmail-style) */
}

/* About quote — agrandi, non-italique, typographie claire */
.about-quote {
  font-size: clamp(20px, 2.1vw, 26px) !important;
  font-style: normal !important;
  font-weight: 400 !important;
  line-height: 1.55 !important;
  padding: 32px 36px !important;
  margin: 0 0 40px !important;
  letter-spacing: -0.005em;
}
@media (max-width: 600px) {
  .about-quote {
    font-size: 18px !important;
    padding: 24px 22px !important;
    line-height: 1.5 !important;
  }
}

/* Nav logo block — name + tagline stacked */
.logo-block {
  display: flex;
  flex-direction: column;
  gap: 2px;
  line-height: 1;
}
.logo-tagline {
  font-family: var(--display);
  font-style: italic;
  font-size: 12px;
  font-weight: 400;
  color: var(--pearl);
  letter-spacing: 0.02em;
  opacity: 0.85;
  margin-top: 2px;
}
@media (max-width: 600px) {
  .logo-tagline {
    font-size: 10px;
    letter-spacing: 0.01em;
    line-height: 1.3;
  }
}
@media (max-width: 380px) {
  .logo-tagline {
    font-size: 9px;
  }
}

/* Pour le titre Avant/Après : R.P.T. était déjà en rose, le · aussi.
   Tout le reste passe en rose maintenant. Aucune surcharge nécessaire. */

/* Inès Kouki en rose au-dessus de "Experte en..." */
.about-photo-name {
  display: block;
  font-family: var(--display);
  font-style: normal;
  font-weight: 600;
  font-size: clamp(22px, 2.4vw, 30px);
  color: var(--terracotta);
  letter-spacing: -0.005em;
  line-height: 1.1;
  margin-bottom: 6px;
}

/* "Inès" / "Inès Kouki" en rose dans la section À propos */
.about-name-rose {
  color: var(--terracotta);
  font-weight: 500;
}

/* ===== RESPONSIVE SAFETY NET ===== */
/* Empêche tout débordement horizontal sur petits écrans */
html, body { overflow-x: hidden; max-width: 100vw; }
img, svg { max-width: 100%; height: auto; }

@media (max-width: 480px) {
  /* Marquees: réduire la taille du texte sur très petit écran */
  .marquee-item { font-size: 14px !important; padding: 0 24px !important; }
  .bridge-item { font-size: 14px !important; }

  /* Stats verticales: empêcher le label de déborder */
  .about-stat-label { font-size: 13px !important; line-height: 1.4 !important; }
  .about-stat-num { font-size: 32px !important; }

  /* Cert title : sur très petit écran, taille réduite */
  .about-cert-title { font-size: 15px !important; line-height: 1.35 !important; }

  /* Photo title sous la photo */
  .about-photo-name { font-size: 19px !important; }
  .about-rpt-letters { font-size: 15px !important; gap: 4px !important; }

  /* R.P.T. definitions list compacte */
  .rpt-def dt { font-size: 19px !important; }
  .rpt-def dd { font-size: 16px !important; }

  /* Bio plus lisible sur mobile */
  .about-body p { font-size: 16px !important; line-height: 1.6 !important; }
}

@media (max-width: 380px) {
  .about-photo-name { font-size: 17px !important; }
  .about-rpt-letters { font-size: 13px !important; }
  .about-rpt-letters .rpt-sep { padding: 0 1px; }
  .about-cert-title { font-size: 13px !important; }
}

@media (max-width: 720px) {
  .dimensions-main-title {
    white-space: normal;
    font-size: clamp(24px, 6vw, 38px) !important;
  }
  .ba-main-title {
    font-size: clamp(20px, 4.6vw, 32px) !important;
  }
  .ba-main-title .ba-arrow {
    margin: 8px 0 !important;
    width: 48px;
  }
}

@media (max-width: 480px) {
  .ba-main-title {
    font-size: clamp(17px, 5vw, 22px) !important;
    padding: 0 8px;
  }
  .ba-main-title .ba-arrow {
    width: 40px;
    margin: 6px 0 !important;
  }
}

/* Hero — remove ambient orbs that create gray haze around CTA */
.hero::before,
.hero::after { display: none !important; }

/* CTA button — remove shimmer overlay for cleaner look */
.btn-primary::after { display: none !important; }

/* CTA button — keep on single line in mobile */
.btn-primary.cta-with-badge {
  white-space: nowrap;
  flex-wrap: nowrap;
}
.btn-primary.cta-with-badge .cta-badge {
  flex-shrink: 0;
}
@media (max-width: 600px) {
  .btn-primary.cta-with-badge {
    font-size: 13px !important;
    padding: 14px 18px !important;
    letter-spacing: 0.06em !important;
  }
  .btn-primary.cta-with-badge .cta-badge {
    font-size: 9px;
    padding: 3px 7px;
    margin-left: 6px;
  }
}
@media (max-width: 380px) {
  .btn-primary.cta-with-badge {
    font-size: 11px !important;
    padding: 12px 14px !important;
  }
}

@media (max-width: 700px) {
  .about-rpt-letters { gap: 6px; font-size: 17px; }
  .rpt-definitions { gap: 16px; margin-top: 28px; }
  .rpt-def { padding-left: 20px; }
}

/* ===========================================================================
   ★ REFONTE DESIGN — Système typographique + photo cadrée + grilles uniformes
   =========================================================================== */

/* --- 1. CONTAINER UNIFORME (toutes sections alignées sur la même grille) --- */
.container {
  max-width: 1200px !important;
  padding-left: 32px !important;
  padding-right: 32px !important;
  margin-left: auto !important;
  margin-right: auto !important;
  width: 100%;
  box-sizing: border-box;
}
@media (max-width: 768px) {
  .container { padding-left: 24px !important; padding-right: 24px !important; }
}
@media (max-width: 480px) {
  .container { padding-left: 20px !important; padding-right: 20px !important; }
}

/* --- 2. SYSTÈME TYPOGRAPHIQUE UNIFIÉ POUR TITRES DE SECTION (-4pt) --- */
/* Toutes les sections partagent la même échelle, plus modeste qu'avant */
.section-title,
.for-who-main-title,
.dimensions-main-title,
.ba-main-title,
.about-eyebrow-large,
.offer-title,
.newsletter-title,
.footer-cta h2,
.dimensions-header h2,
.discovery-inner h2,
.who-is-text h2 {
  font-size: clamp(28px, 4vw, 56px) !important;
  line-height: 1.15 !important;
  letter-spacing: -0.015em !important;
  margin-bottom: 28px !important;
}

/* Sous-titre R.P.T. — proportionnel mais distinct */
.dimensions-subtitle {
  font-size: clamp(20px, 2.4vw, 32px) !important;
  line-height: 1.35 !important;
  margin-bottom: 28px !important;
}

/* Hero H1 — grand titre signature, calibré -4pt */
.hero h1 {
  font-size: clamp(32px, 6.5vw, 72px) !important;
  line-height: 1.1 !important;
  letter-spacing: -0.025em !important;
}

/* About title (signature "Je clarifie...") — légèrement plus petit */
.about-title {
  font-size: clamp(28px, 4vw, 52px) !important;
  line-height: 1.15 !important;
}

/* Body / paragraphes — taille fluide cohérente */
.about-body p,
.hero-promise,
.hero-sub,
.section-intro,
.offer-desc {
  font-size: clamp(16px, 1.5vw, 19px) !important;
  line-height: 1.7 !important;
}

/* --- 3. PHOTO INÈS — petit cadre net et lisible --- */
.about-wrapper {
  display: grid !important;
  grid-template-columns: 360px 1fr !important;
  gap: 64px !important;
  align-items: start !important;
  max-width: 1100px;
  margin: 0 auto;
}
.about-photo-col {
  width: 360px !important;
  height: auto !important;
  position: sticky;
  top: 80px;
}
.about-photo-inner {
  width: 320px !important;
  height: 400px !important;
  margin: 0 auto;
  border-radius: 4px;
  overflow: hidden;
  position: relative;
  border: 1px solid rgba(196, 120, 154, 0.25);
  box-shadow:
    0 24px 48px rgba(0, 0, 0, 0.35),
    0 0 0 8px rgba(28, 16, 48, 0.4),
    0 0 0 9px rgba(196, 120, 154, 0.15);
}
.about-photo-inner img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  object-position: center 20% !important;
  filter: saturate(0.95) contrast(1.05) !important;
}
/* Réduire le gradient sombre qui assombrit le visage */
.about-photo-inner::after {
  background: linear-gradient(
    180deg,
    rgba(28,16,48,0) 0%,
    rgba(28,16,48,0) 60%,
    rgba(28,16,48,0.5) 100%
  ) !important;
}
.about-photo-line { display: none !important; }

/* Stats sous la photo */
.about-stats {
  width: 320px !important;
  margin: 24px auto 0 !important;
  padding: 0 !important;
  position: static !important;
}
.about-stat {
  padding: 12px 0 !important;
  border-bottom: 1px solid rgba(250, 247, 242, 0.08);
  display: flex;
  align-items: baseline;
  gap: 16px;
}
.about-stat:last-child { border-bottom: none; }
.about-stat-num {
  font-size: 28px !important;
  flex-shrink: 0;
}
.about-stat-label {
  font-size: 13px !important;
  line-height: 1.4 !important;
}

/* Photo title sous la photo, aligné avec le cadre */
.about-photo-title {
  width: 320px !important;
  margin: 16px auto 0 !important;
  text-align: center;
}
.about-photo-name {
  font-size: clamp(20px, 1.8vw, 24px) !important;
}
.about-rpt-letters {
  font-size: clamp(13px, 1.3vw, 16px) !important;
}

/* Cert title et certs alignés */
.about-cert-title {
  font-size: clamp(15px, 1.5vw, 18px) !important;
}

/* --- 4. TEXTE JUSTIFIÉ DANS LES BLOCS DE PARAGRAPHES --- */
.about-body p,
.offer-desc,
.section-intro {
  text-align: justify;
  hyphens: auto;
  -webkit-hyphens: auto;
}

/* --- 5. RESPONSIVE : grille à 1 colonne sous 900px, photo centrée --- */
@media (max-width: 900px) {
  .about-wrapper {
    grid-template-columns: 1fr !important;
    gap: 40px !important;
  }
  .about-photo-col {
    width: 100% !important;
    position: static !important;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .about-photo-inner,
  .about-stats,
  .about-photo-title {
    margin-left: auto !important;
    margin-right: auto !important;
  }
  .about-content-col { text-align: left; }
}

@media (max-width: 480px) {
  .about-photo-inner {
    width: 280px !important;
    height: 350px !important;
  }
  .about-stats,
  .about-photo-title { width: 280px !important; }

  /* Justification désactivée sur mobile (rivières typographiques) */
  .about-body p,
  .offer-desc,
  .section-intro {
    text-align: left;
  }
}

/* --- 6. ESPACEMENT VERTICAL UNIFORME ENTRE SECTIONS --- */
.who-is,
.dimensions,
.for-who,
.before-after,
.offer,
.newsletter-section,
.footer-cta {
  padding-top: clamp(80px, 9vw, 120px) !important;
  padding-bottom: clamp(80px, 9vw, 120px) !important;
}
@media (max-width: 600px) {
  .who-is, .dimensions, .for-who, .before-after,
  .offer, .newsletter-section, .footer-cta {
    padding-top: 64px !important;
    padding-bottom: 64px !important;
  }
}

/* --- 7. RESPONSIVE NAV : tagline visible sur tous écrans, ajustée mobile --- */
.nav-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
  flex-wrap: wrap;
}
@media (max-width: 600px) {
  .nav-inner {
    gap: 12px;
  }
  .logo {
    font-size: 20px !important;
  }
}
@media (max-width: 420px) {
  .logo-tagline {
    font-size: 9px !important;
    letter-spacing: 0;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    max-width: 100%;
  }
  .logo {
    font-size: 18px !important;
  }
}

/* --- 8. BOUTON CTA "DISCOVERY" — responsive dédié (texte plus long) --- */
/* Sur la section Appel découverte 45 min, le bouton "Réserver notre premier
   échange (gratuit)" a besoin d'un traitement responsive spécifique car le
   texte est plus long et le contexte (centré dans une carte) est différent. */
.discovery-cta {
  display: inline-flex !important;
  align-items: center;
  justify-content: center;
  gap: 10px !important;
  flex-wrap: nowrap !important;
  white-space: nowrap;
  text-align: center;
  margin-top: 28px !important;
  max-width: 100%;
  box-sizing: border-box;
}
.discovery-cta .cta-badge {
  flex-shrink: 0;
}

/* Tablette : taille intermédiaire */
@media (max-width: 720px) {
  .discovery-cta {
    font-size: 14px !important;
    padding: 14px 24px !important;
    letter-spacing: 0.05em !important;
    min-height: 48px !important;
  }
  .discovery-cta .cta-badge {
    font-size: 9px !important;
    padding: 3px 8px !important;
    margin-left: 6px !important;
  }
}

/* Mobile standard : passe sur 2 lignes (texte / badge) pour rester lisible */
@media (max-width: 480px) {
  .discovery-cta {
    flex-wrap: wrap !important;
    flex-direction: column !important;
    gap: 8px !important;
    white-space: normal;
    width: 100%;
    max-width: 320px;
    padding: 16px 20px !important;
    font-size: 13px !important;
    line-height: 1.3 !important;
    letter-spacing: 0.06em !important;
  }
  .discovery-cta .cta-badge {
    font-size: 9px !important;
    padding: 2px 10px !important;
    margin-left: 0 !important;
  }
  .discovery-inner {
    padding: 32px 20px !important;
  }
}

/* Mobile très petit */
@media (max-width: 360px) {
  .discovery-cta {
    font-size: 12px !important;
    padding: 14px 16px !important;
    letter-spacing: 0.04em !important;
  }
}


/* ===== AMPERSANDS STYLISÉS ===== */
.ba-ampersand,
.about-ampersand,
.logo-amp {
  font-family: 'EB Garamond', Georgia, serif;
  font-style: italic;
  font-weight: 400;
  color: var(--terracotta);
  font-size: 0.9em;
  letter-spacing: 0;
  display: inline-block;
  margin: 0 3px;
  line-height: 1;
  vertical-align: baseline;
}
.ba-ampersand {
  font-size: 0.9em;
}
.logo-amp {
  font-size: 0.85em;
  margin: 0 2px;
}

/* ===== PHOTO INÈS — RESPONSIVE RENFORCÉ ===== */
/* Sur mobile: la photo prend toute la largeur disponible,
   cadrage tête bien visible (object-position haut) */
@media (max-width: 768px) {
  .about-photo-inner {
    width: min(560px, 96vw) !important;
    height: min(560px, 96vw) !important;
    margin: 0 auto !important;
    border-radius: 4px !important;
    overflow: hidden;
    box-shadow:
      0 24px 48px rgba(0,0,0,0.4),
      0 0 0 6px rgba(28,16,48,0.5),
      0 0 0 7px rgba(196,120,154,0.18) !important;
  }
  .about-photo-inner img {
    object-fit: cover !important;
    object-position: center 15% !important;
    width: 100% !important;
    height: 100% !important;
    filter: saturate(1.05) contrast(1.05) brightness(1.02) !important;
  }
  .about-photo-inner::after {
    background: linear-gradient(
      180deg,
      rgba(28,16,48,0) 0%,
      rgba(28,16,48,0) 55%,
      rgba(28,16,48,0.4) 100%
    ) !important;
  }
  .about-photo-col {
    display: flex !important;
    flex-direction: column !important;
    align-items: center !important;
    gap: 20px !important;
    height: auto !important;
  }
  .about-photo-title,
  .about-stats {
    width: min(560px, 96vw) !important;
    margin: 0 auto !important;
  }
}

@media (max-width: 480px) {
  .about-photo-inner {
    width: 96vw !important;
    height: 96vw !important;
  }
  .about-photo-title,
  .about-stats {
    width: 96vw !important;
  }
  .about-photo-name {
    font-size: 20px !important;
  }
  .about-rpt-letters {
    font-size: 14px !important;
  }
}

@media (max-width: 360px) {
  .about-photo-inner {
    width: 94vw !important;
    height: 94vw !important;
  }
  .about-photo-title,
  .about-stats {
    width: 94vw !important;
  }
}

/* ===== BADGE CTA RESPONSIVE ===== */
/* S'assure que le bouton a assez de padding en haut pour que le badge ne soit pas coupé */
.btn-primary.cta-with-badge {
  padding-top: 18px !important;
  margin-top: 20px;
}
@media (max-width: 600px) {
  .cta-with-badge .cta-badge {
    right: 12px !important;
    font-size: 8px !important;
    top: -12px !important;
    padding: 3px 8px !important;
  }
}

</style>
</head>

<body>

<!-- NAV -->
<nav class="nav">
  <div class="nav-inner">
    <div class="logo-block">
      <div class="logo">Inès <span>Kouki</span></div>
      <div class="logo-tagline">Experte en Rôle, Posture et Trajectoire</div>
    </div>
    <div class="nav-tag">R.P.T. · Rôle · Posture · Trajectoire</div>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="container">
    <div class="hero-content">

      <h1 class="fade-up d2">
        De la confusion professionnelle<br>
        à la <em>clarté stratégique</em>
      </h1>

      <p class="hero-sub fade-up d3">
        Vous avancez <strong>mais vous stagnez.</strong><br>
        Vous vous adaptez <strong>mais vous ne pilotez pas.</strong>
      </p>

      <div class="hero-divider fade-up d3"></div>

      <p class="hero-promise fade-up d3">
        « Je transforme le flou de rôle en position claire, visible et évolutive. Parlons-en. »
      </p>

      <div class="hero-cta-group fade-up d4">
        <button class="btn-primary cta-with-badge" onclick="window.open('https://calendly.com/ines-kouki-yb9r/30min','_blank')">
          Réserver notre premier échange <span class="cta-badge">Gratuit</span>
        </button>
      </div>

    </div>
  </div>

</section>

<!-- MARQUEE -->
<div class="marquee-strip">
  <div class="marquee-track">
    <div class="marquee-item">Rôle clair</div>
    <div class="marquee-item">Posture affirmée</div>
    <div class="marquee-item">Trajectoire pilotée</div>
    <div class="marquee-item">17 ans en transformation complexe</div>
    <div class="marquee-item">4 Continents</div>
    <div class="marquee-item">SAFe SPC · ICP-ACC</div>
    <div class="marquee-item">Banque · Retail · Sécurité Numérique</div>
    <div class="marquee-item">Rôle clair</div>
    <div class="marquee-item">Posture affirmée</div>
    <div class="marquee-item">Trajectoire pilotée</div>
    <div class="marquee-item">17 ans en transformation complexe</div>
    <div class="marquee-item">4 Continents</div>
    <div class="marquee-item">SAFe SPC · ICP-ACC</div>
    <div class="marquee-item">Banque · Retail · Sécurité Numérique</div>
  </div>
</div>

<!-- DISCOVERY CALL -->
<section class="discovery">
  <div class="container">
    <div class="discovery-inner">
      <h2>Appel découverte — 45 minutes</h2>
      <p>Un échange de 45 minutes pour clarifier votre rôle, votre posture et votre trajectoire.</p>
      <p>Une conversation pour voir si le Diagnostic R.P.T. est fait pour vous.</p>
      <p>Après cet appel, vous déciderez librement.</p>

    </div>
  </div>
</section>

<!-- FOR WHO -->
<section class="for-who">
  <div class="container">
    <h2 class="section-title for-who-main-title">Vous vous reconnaissez ?</h2>
    <p class="for-who-subtitle">Une (ou plusieurs) de ces situations vous ressemblent ?</p>

    <div class="situations-grid">
      <div class="situation">
        <div class="situation-number">01</div>
        <h3>Votre rôle a changé</h3>
        <p>Ce que votre rôle demande a changé. Vous ne savez pas si vos compétences d'hier suffisent encore dans la nouvelle configuration.</p>
      </div>

      <div class="situation">
        <div class="situation-number">02</div>
        <h3>Vous stagnez malgré votre compétence</h3>
        <p>Vous délivrez. Votre manager le sait. Mais les opportunités passent à côté de vous. Vous voyez des collègues moins expérimentés progresser plus vite. Ce n'est pas une question de compétence.</p>
      </div>

      <div class="situation">
        <div class="situation-number">03</div>
        <h3>Votre expertise devient obsolète ?</h3>
        <p>L'IA s'installe. Les transformations s'enchaînent. Vous vous demandez : ce que je sais faire aujourd'hui vaudra-t-il encore dans 12 mois ?</p>
      </div>

      <div class="situation">
        <div class="situation-number">04</div>
        <h3>Vous ne savez pas où vous allez</h3>
        <p>Vous enchaînez les missions sans les avoir choisies. Vous adaptez votre identité pour matcher les besoins. Vous réagissez. Vous ne pilotez pas.</p>
      </div>

      <div class="situation">
        <div class="situation-number">05</div>
        <h3>Votre valeur réelle est invisible</h3>
        <p>Vous portez beaucoup : coordination, facilitation, résolution de tensions. Cette contribution est rarement formalisée et encore moins reconnue aux bons endroits.</p>
      </div>

      <div class="situation situation-bridge">
        <div class="situation-number">06</div>
        <h3>Vous reconnaissez ce qui se joue</h3>
        <p>Le cadre de diagnostic R.P.T. répond précisément à ces situations. Trois dimensions, un seul objectif&nbsp;: votre clarté stratégique.</p>
      </div>
    </div>
  </div>
</section>

<!-- RPT DIMENSIONS -->
<section class="dimensions">
  <div class="container">
    <div class="dimensions-header">
      <h2 class="section-title dimensions-main-title">Le cadre du diagnostic</h2>
      <p class="dimensions-subtitle">R.P.T. un diagnostic systémique en trois dimensions.<br>Un seul objectif&nbsp;: votre clarté stratégique.</p>
      <p>Les organisations investissent massivement dans les méthodes. Moins dans la clarté des rôles, la posture et les trajectoires des individus qui portent réellement la transformation.</p>
      <p class="lead">« La transformation échoue rarement par manque de méthode.<br>Elle échoue quand les rôles sont flous, les postures fragiles et les trajectoires subies. »</p>
    </div>

    <div class="pillars-grid">
      <!-- R -->
      <div class="pillar">
        <div class="pillar-accent"></div>
        <div class="pillar-letter">R</div>
        <h2 class="pillar-title">Rôle</h2>
        <p class="pillar-subtitle">Clarifier votre valeur réelle dans le système</p>
        <p class="pillar-intro">Dans les transformations, les titres sont trompeurs. Le rôle réel ≠ le titre officiel. Comprendre ce que vous apportez vraiment, pas ce que votre fiche de poste dit, ça change tout.</p>
        <ul class="pillar-questions">
          <li>Quel problème réel résolvez-vous dans ce système ?</li>
          <li>Où se situe votre périmètre d'influence réel ?</li>
          <li>Qu'est-ce que vous devez lâcher et ajouter ?</li>
        </ul>
        <div class="pillar-benefit">
          ✓ Fin du flou professionnel
          <em>Vous savez ce que vous apportez et où vous créez de l'impact.</em>
        </div>
      </div>

      <!-- P -->
      <div class="pillar">
        <div class="pillar-accent"></div>
        <div class="pillar-letter">P</div>
        <h2 class="pillar-title">Posture</h2>
        <p class="pillar-subtitle">S'affirmer sans sur-effort</p>
        <p class="pillar-intro">Deux personnes avec le même rôle peuvent avoir des impacts opposés. La différence n'est pas la compétence. C'est la posture : présence, autorité naturelle, capacité d'influence.</p>
        <ul class="pillar-questions">
          <li>Comment êtes-vous perçue face au pouvoir et aux décisions ?</li>
          <li>Comment développer une autorité naturelle sans surjouer ?</li>
          <li>Comment vous affirmer dans les dynamiques invisibles ?</li>
        </ul>
        <div class="pillar-benefit">
          ✓ Influence sans surjouer
          <em>Vous occupez votre place avec clarté et crédibilité perçue.</em>
        </div>
      </div>

      <!-- T -->
      <div class="pillar">
        <div class="pillar-accent"></div>
        <div class="pillar-letter">T</div>
        <h2 class="pillar-title">Trajectoire</h2>
        <p class="pillar-subtitle">Piloter, pas subir</p>
        <p class="pillar-intro">Beaucoup de professionnels vivent mission après mission sans direction claire. Fatigue, stagnation, perte de sens. La trajectoire se construit intentionnellement ou elle vous échappe.</p>
        <ul class="pillar-questions">
          <li>Où cette expérience vous emmène-t-elle vraiment ?</li>
          <li>Comment choisir la prochaine étape intentionnellement ?</li>
          <li>Comment construire une cohérence long terme ?</li>
        </ul>
        <div class="pillar-benefit">
          ✓ Carrière pilotée, non subie
          <em>Vous avez un cap clair et une stratégie pour l'atteindre.</em>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- AVANT / APRÈS -->
<section class="before-after">
  <div class="container">
    <div class="before-after-header">
      <h2 class="section-title ba-main-title">Avant et Après le diagnostic <span class="ba-rpt">R.P.T.</span></h2>
      <p class="ba-subtitle">Vos 5 problèmes — Vos 5 réponses concrètes</p>
    </div>

    <div class="ba-grid">
      <div class="ba-row">
        <div class="ba-cell before">
          <div class="ba-label">Avant Diagnostic (R.P.T.)</div>
          <div class="ba-problem">« Mon rôle a changé. Je ne sais plus où je me situe. »</div>
        </div>
        <div class="ba-cell after">
          <div class="ba-label">Après Diagnostic (R.P.T.)</div>
          <div class="ba-solution">
            <span class="key">L'écart exact entre votre expertise actuelle et la demande</span>
            <span>Ce que vous devez lâcher et ce que vous devez ajouter</span>
            <span>Votre valeur réelle dans la nouvelle configuration</span>
          </div>
        </div>
      </div>

      <div class="ba-row">
        <div class="ba-cell before">
          <div class="ba-label">Avant Diagnostic (R.P.T.)</div>
          <div class="ba-problem">« Je stagne malgré ma compétence. Je ne comprends pas pourquoi. »</div>
        </div>
        <div class="ba-cell after">
          <div class="ba-label">Après Diagnostic (R.P.T.)</div>
          <div class="ba-solution">
            <span class="key">Pourquoi vous stagnez alors que vous travaillez bien</span>
            <span>Ce qui se joue dans les dynamiques invisibles autour de vous</span>
            <span>Comment vous rendre visible aux bons endroits</span>
          </div>
        </div>
      </div>

      <div class="ba-row">
        <div class="ba-cell before">
          <div class="ba-label">Avant Diagnostic (R.P.T.)</div>
          <div class="ba-problem">« L'IA arrive. L'anxiété monte. Et si ce que je sais faire n'était plus utile ? »</div>
        </div>
        <div class="ba-cell after">
          <div class="ba-label">Après Diagnostic (R.P.T.)</div>
          <div class="ba-solution">
            <span class="key">Ce qui fait votre vraie valeur (au-delà des outils)</span>
            <span>Comment vous restez pertinente, intentionnellement</span>
          </div>
        </div>
      </div>

      <div class="ba-row">
        <div class="ba-cell before">
          <div class="ba-label">Avant Diagnostic (R.P.T.)</div>
          <div class="ba-problem">« J'enchaîne les missions sans construire de trajectoire. »</div>
        </div>
        <div class="ba-cell after">
          <div class="ba-label">Après Diagnostic (R.P.T.)</div>
          <div class="ba-solution">
            <span class="key">Votre trajectoire pilotée (vs. subie)</span>
            <span>La prochaine étape choisie intentionnellement, pas par défaut</span>
          </div>
        </div>
      </div>

      <div class="ba-row">
        <div class="ba-cell before">
          <div class="ba-label">Avant Diagnostic (R.P.T.)</div>
          <div class="ba-problem">« Je contribue énormément. Mais ça ne se voit pas. »</div>
        </div>
        <div class="ba-cell after">
          <div class="ba-label">Après Diagnostic (R.P.T.)</div>
          <div class="ba-solution">
            <span class="key">Votre contribution rendue visible et défendable</span>
            <span>Comment positionner cette valeur en interne comme en externe</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- WHO IS INÈS -->
<section class="who-is">
  <div class="about-wrapper">

    <!-- Photo — colonne gauche -->
    <div class="about-photo-col">
      <div class="about-photo-inner">
        <img src="data:image/webp;base64,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" alt="Inès Kouki — Consultante en transformation agile">

        <div class="about-photo-line"></div>
        <div class="about-photo-title">
          <span class="about-photo-name">Inès Kouki</span>
          <span class="about-photo-title-prefix">Experte en</span>
          <span class="about-rpt-letters">
            <span class="rpt-r">Rôle</span><span class="rpt-sep">,</span>
            <span class="rpt-p">Posture</span><span class="rpt-sep">et</span>
            <span class="rpt-t">Trajectoire</span>
          </span>
        </div>
      </div>

      <!-- Stats verticales -->
      <div class="about-stats">
        <div class="about-stat">
          <div class="about-stat-num">4</div>
          <div class="about-stat-label">Continents</div>
        </div>
        <div class="about-stat">
          <div class="about-stat-num">3</div>
          <div class="about-stat-label">Secteurs d'activités · Banque · Retail · Sécurité Numérique</div>
        </div>
      </div>
    </div>

    <!-- Contenu — colonne droite -->
    <div class="about-content-col">
      <div class="about-eyebrow about-eyebrow-large">À propos d'<span class="about-name-rose">Inès</span></div>

      <h2 class="about-title">
        Je clarifie<br>
        ce que les <span class="about-frameworks">frameworks</span><br>
        ne clarifient jamais.
      </h2>

      <div class="about-divider-h"></div>

      <div class="about-body">
        <p>J'ai grandi entre cultures et appris à naviguer dans des environnements multiculturels. Mes missions au sein des organisations internationales (<a href="https://www.linkedin.com/company/1912/" target="_blank" rel="noopener" style="color:inherit;text-decoration:none;">Philip Morris International</a>, IDEMIA, Société Générale et BNP Paribas) m'ont permis de voir ce que peu voient.</p>

        <p>4 pays. 3 secteurs d'activités. À chaque transition, j'ai dû décoder les règles non écrites&nbsp;: comment m'affirmer, être vue, rester pertinente quand tout autour se reconfigure.</p>

        <p>J'ai commencé par le marketing, où j'ai appris à comprendre les personnes, créer de l'adhésion et traduire la complexité en clarté. Ces compétences sont devenues le cœur de mon approche R.P.T&nbsp;:</p>

        <dl class="rpt-definitions">
          <div class="rpt-def rpt-def-r">
            <dt><span class="rpt-letter">R</span><span class="rpt-word">ÔLE</span></dt>
            <dd>Qu'est-ce que vous faites vraiment&nbsp;?</dd>
          </div>
          <div class="rpt-def rpt-def-p">
            <dt><span class="rpt-letter">P</span><span class="rpt-word">OSTURE</span></dt>
            <dd>Comment êtes-vous perçue&nbsp;?</dd>
          </div>
          <div class="rpt-def rpt-def-t">
            <dt><span class="rpt-letter">T</span><span class="rpt-word">RAJECTOIRE</span></dt>
            <dd>Où allez-vous réellement&nbsp;?</dd>
          </div>
        </dl>
      </div>

      <blockquote class="about-quote">
        « La transformation ne réussit pas grâce aux méthodes seulement. Elle réussit quand les acteurs clés savent clairement quelle est leur place, et la place qu'ils veulent construire. »
      </blockquote>

      <!-- Certifications -->
      <div class="about-certs">
        <div class="about-cert-title"><span class="about-name-rose">Inès Kouki</span> — Experte en Rôle, Posture et Trajectoire</div>
        <span class="about-cert-label">Certifiée</span>
        <div class="about-cert-badges">
          <span class="about-cert">SAFe SPC®</span>
          <span class="about-cert-dot">·</span>
          <span class="about-cert">ICP-ACC</span>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- BRIDGE MARQUEE — between À propos and Offer -->
<div class="marquee-strip marquee-bridge">
  <div class="marquee-track">
    <div class="marquee-item bridge-item">Notre premier échange (sans engagement)</div>
    <div class="marquee-item bridge-item">★</div>
    <div class="marquee-item bridge-item">Vous décidez si vous souhaitez aller plus loin avec le diagnostic complet R.P.T.</div>
    <div class="marquee-item bridge-item">★</div>
    <div class="marquee-item bridge-item">Notre premier échange (sans engagement)</div>
    <div class="marquee-item bridge-item">★</div>
    <div class="marquee-item bridge-item">Vous décidez si vous souhaitez aller plus loin avec le diagnostic complet R.P.T.</div>
    <div class="marquee-item bridge-item">★</div>
  </div>
</div>

<!-- OFFER -->
<section class="offer">
  <div class="container">
    <div class="offer-card">
      <h2 class="offer-title">Diagnostic R.P.T.</h2>
      <div class="offer-badge">Diagnostic systémique · Rôle · Posture · Trajectoire</div>

      <p class="offer-desc">3 à 4 sessions de travail de 1h30 + analyse approfondie entre les sessions.</p>
      <p class="offer-desc"><strong>Ce que vous recevez :</strong></p>

      <ul class="offer-list">
        <li>Cartographie de votre rôle réel dans votre contexte de transformation</li>
        <li>Analyse de votre posture : ce qui fonctionne et ce qui vous freine</li>
        <li>Trajectoire clarifiée : la prochaine étape choisie, pas subie</li>
        <li>Plan d'action sur 90 jours, applicable dès la dernière session</li>
      </ul>


    </div>
  </div>
</section>

<!-- FOOTER CTA -->
<section class="footer-cta">
  <div class="container">
    <h2>Vous savez que quelque chose doit changer<br>Commençons par un appel découverte</h2>
    <p>45 minutes pour clarifier si vous êtes prête à travailler votre rôle, votre posture et votre trajectoire</p>
    <a href="https://calendly.com/ines-kouki-yb9r/30min" target="_blank" class="btn-primary cta-with-badge">Réserver notre premier échange <span class="cta-badge">Gratuit</span></a>
  </div>
</section>

<!-- NEWSLETTER -->
<section class="newsletter-section">
  <div class="container">
    <div class="newsletter-card">
      <div class="newsletter-eyebrow">Communauté · LinkedIn Newsletter</div>
      <h2 class="newsletter-title">
        <span class="newsletter-linkedin-icon" aria-hidden="true">
          <svg width="36" height="36" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        </span>
        Rejoignez la communauté <span class="newsletter-decoding">«&nbsp;Decoding the System&nbsp;»</span>
      </h2>
      <p class="newsletter-desc">Une lecture stratégique des dynamiques invisibles dans les organisations en transformation. Pour celles et ceux qui veulent comprendre ce qui se joue vraiment derrière les méthodes.</p>
      <a href="https://www.linkedin.com/newsletters/decoding-the-system-7454113581735833600/" target="_blank" rel="noopener" class="btn-primary newsletter-cta">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor" style="margin-right:10px;"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        S'inscrire à la newsletter
      </a>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer class="footer">
  <div class="container">
    <div class="footer-inner footer-inner-split">
      <div class="footer-links footer-links-left">
        <a href="https://www.linkedin.com/in/ines-kouki-ik/" target="_blank" rel="noopener" class="footer-link">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
          LinkedIn
        </a>
        <a href="mailto:ines.kouki@outlook.com" class="footer-link">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,12 2,6"/></svg>
          Email
        </a>
      </div>
      <div class="footer-links footer-links-right">
      </div>
    </div>
    <div class="footer-copy footer-copy-bottom">
      © 2026 Inès Kouki · R.P.T. — Rôle · Posture · Trajectoire
    </div>
  </div>
</footer>


<!-- ─── BOUTON WHATSAPP FLOTTANT ─── -->
<a 
  href="https://wa.me/33631805966?text=Bonjour%20In%C3%A8s%2C%20j%27ai%20visit%C3%A9%20votre%20site%20et%20je%20souhaite%20en%20savoir%20plus%20sur%20le%20Diagnostic%20R.P.T." 
  target="_blank" 
  rel="noopener noreferrer"
  class="whatsapp-btn" 
  aria-label="Contacter Inès sur WhatsApp"
>
  <div class="whatsapp-icon">
    <svg width="28" height="28" viewBox="0 0 24 24" fill="white" xmlns="http://www.w3.org/2000/svg">
      <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/>
    </svg>
  </div>
  <span class="whatsapp-label">Écrire sur WhatsApp</span>
  <div class="whatsapp-pulse"></div>
</a>

</body>
</html>
