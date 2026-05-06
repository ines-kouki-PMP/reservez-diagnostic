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
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">

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
.cta-with-badge .cta-badge {
  display: inline-block;
  background: var(--cream);
  color: var(--midnight);
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  font-weight: 700;
  padding: 4px 10px;
  margin-left: 10px;
  border-radius: 999px;
  vertical-align: middle;
  position: relative;
  animation: cta-badge-float 2.4s ease-in-out infinite;
  box-shadow: 0 4px 12px rgba(196, 120, 154, 0.35);
}
@keyframes cta-badge-float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-3px); }
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
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
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
  color: rgba(196,120,154,0.2);
  margin-bottom: 20px;
  transition: color 0.3s;
}
.situation:hover .situation-number { color: rgba(196,120,154,0.5); }

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
  .situations-grid { grid-template-columns: 1fr; }
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
  .situations-grid { grid-template-columns: 1fr; }
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
  }
}
@media (max-width: 380px) {
  .logo-tagline {
    display: none;
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

</style>
</head>

<body>

<!-- NAV -->
<nav class="nav">
  <div class="nav-inner">
    <div class="logo-block">
      <div class="logo">Inès <span>Kouki</span></div>
      <div class="logo-tagline">Experte en Rôle, Posture &amp; Trajectoire</div>
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
        Vous portez des programmes complexes.<br>
        <strong>Mais votre propre trajectoire reste floue.</strong>
      </p>

      <div class="hero-divider fade-up d3"></div>

      <p class="hero-promise fade-up d3">
        « Je transforme le flou de rôle en position claire, visible et évolutive. Parlons-en. »
      </p>

      <div class="hero-cta-group fade-up d4">
        <button class="btn-primary cta-with-badge" onclick="window.open('https://calendly.com/ines-kouki-yb9r/30min','_blank')">
          Réserver notre premier échange <span class="cta-badge">gratuit</span>
        </button>
      </div>

    </div>
  </div>

</section>

<!-- MARQUEE -->
<div class="marquee-strip">
  <div class="marquee-track">
    <div class="marquee-item">Clarté de Rôle</div>
    <div class="marquee-item">Posture Professionnelle</div>
    <div class="marquee-item">Trajectoire de Carrière</div>
    <div class="marquee-item">17 Ans en Transformation</div>
    <div class="marquee-item">4 Continents</div>
    <div class="marquee-item">SAFe SPC · ICP-ACC</div>
    <div class="marquee-item">Banque · Retail · Sécurité Numérique</div>
    <div class="marquee-item">Clarté de Rôle</div>
    <div class="marquee-item">Posture Professionnelle</div>
    <div class="marquee-item">Trajectoire de Carrière</div>
    <div class="marquee-item">17 Ans en Transformation</div>
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
      <p>Parlons de votre situation actuelle</p>
      <p>Une conversation pour clarifier si le Diagnostic R.P.T. est fait pour vous</p>
      <a href="https://calendly.com/ines-kouki-yb9r/30min" target="_blank" rel="noopener noreferrer" class="btn-primary cta-with-badge discovery-cta">Réserver notre premier échange <span class="cta-badge">gratuit</span></a>
    </div>
  </div>
</section>

<!-- FOR WHO -->
<section class="for-who">
  <div class="container">
    <h2 class="section-title for-who-main-title">Vous reconnaissez-vous ?</h2>
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
      <h2 class="section-title dimensions-main-title">Le cadre de diagnostic</h2>
      <p class="dimensions-subtitle">R.P.T. — Un diagnostic systémique en trois dimensions.<br>Un seul objectif&nbsp;: votre clarté stratégique.</p>
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
      <h2 class="section-title ba-main-title">Avant Diagnostic <span class="ba-rpt">R.P.T.</span> <span class="ba-arrow">·</span> Après Diagnostic <span class="ba-rpt">R.P.T.</span></h2>
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
            <span class="key">✓ L'écart exact entre votre expertise actuelle et la demande</span>
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
            <span class="key">✓ Pourquoi vous stagnez alors que vous travaillez bien</span>
            <span>Ce qui se joue dans les dynamiques invisibles autour de vous</span>
            <span>Comment vous rendre visible aux bons endroits</span>
          </div>
        </div>
      </div>

      <div class="ba-row">
        <div class="ba-cell before">
          <div class="ba-label">Avant Diagnostic (R.P.T.)</div>
          <div class="ba-problem">« L'IA arrive. Je ne sais pas si mon expertise restera pertinente. »</div>
        </div>
        <div class="ba-cell after">
          <div class="ba-label">Après Diagnostic (R.P.T.)</div>
          <div class="ba-solution">
            <span class="key">✓ Ce qui vous rend indispensable dans la transformation technologique</span>
            <span>Votre stratégie pour rester pertinente à 18 mois</span>
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
            <span class="key">✓ Votre trajectoire pilotée (vs. subie)</span>
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
            <span class="key">✓ Votre contribution rendue visible et défendable</span>
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
        <img src="data:image/jpeg;base64,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" alt="Inès Kouki — Consultante en transformation agile">

        <div class="about-photo-line"></div>
        <div class="about-photo-title">
          <span class="about-photo-name">Inès Kouki</span>
          <span class="about-photo-title-prefix">Experte en</span>
          <span class="about-rpt-letters">
            <span class="rpt-r">Rôle</span><span class="rpt-sep">,</span>
            <span class="rpt-p">Posture</span><span class="rpt-sep">&amp;</span>
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
        <div class="about-stat">
          <div class="about-stat-num">+100</div>
          <div class="about-stat-label">Professionnels accompagnés</div>
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
        <p>J'ai grandi entre cultures et appris à naviguer dans des environnements multiculturels. Mes missions au sein des organisations internationales (<a href="https://www.linkedin.com/company/1912/" target="_blank" rel="noopener" class="about-link"><strong>Philip Morris International</strong></a>, <strong>IDEMIA</strong>, <strong>Société Générale</strong> et <strong>BNP Paribas</strong>) m'ont permis de voir ce que peu voient.</p>

        <p>4 pays. 3 secteurs d'activités. À chaque transition, j'ai dû décoder les règles non écrites&nbsp;: comment m'affirmer, être vue, rester pertinente quand tout autour se reconfigure.</p>

        <p>J'ai commencé par le <strong>marketing</strong>, où j'ai appris à comprendre les personnes, créer de l'adhésion et traduire la complexité en clarté. Ces compétences sont devenues le cœur de mon approche R.P.T&nbsp;:</p>

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
        <div class="about-cert-title"><span class="about-name-rose">Inès Kouki</span> — Experte en Rôle, Posture &amp; Trajectoire</div>
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
    <div class="marquee-item bridge-item">Après notre premier échange (Gratuit, sans engagement)</div>
    <div class="marquee-item bridge-item">★</div>
    <div class="marquee-item bridge-item">Vous décidez si vous souhaitez aller plus loin avec le diagnostic complet R.P.T.</div>
    <div class="marquee-item bridge-item">★</div>
    <div class="marquee-item bridge-item">Après notre premier échange (Gratuit, sans engagement)</div>
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
    <a href="https://calendly.com/ines-kouki-yb9r/30min" target="_blank" class="btn-primary cta-with-badge">Réserver notre premier échange <span class="cta-badge">gratuit</span></a>
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
