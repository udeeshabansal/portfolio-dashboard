# portfolio-dashboard
[portfolio.html](https://github.com/user-attachments/files/35258572/portfolio.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Udeesha Bansal | Strategy · Analytics · Decisions</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Newsreader:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
<style>
:root{--bg:#0C0C0C;--bg-card:#161616;--bg-ev:#1C1C1C;--fg:#F0EFEB;--fg-mid:#A8A8A2;--fg-dim:#666660;--accent:#E8503A;--accent-glow:rgba(232,80,58,.12);--green:#3CB88C;--green-dim:rgba(60,184,140,.12);--border:#2A2A28;--display:'Space Grotesk',system-ui,sans-serif;--body:'Newsreader',Georgia,serif;color-scheme:dark}
@media(prefers-color-scheme:light){:root:not([data-theme="dark"]){--bg:#F8F7F4;--bg-card:#FFF;--bg-ev:#F0EFEB;--fg:#1A1A18;--fg-mid:#5A5A56;--fg-dim:#9A9A94;--accent:#D04030;--accent-glow:rgba(208,64,48,.08);--green:#1B8A60;--green-dim:rgba(27,138,96,.08);--border:#E0DFDA;color-scheme:light}}
*{margin:0;padding:0;box-sizing:border-box}html{scroll-behavior:smooth;scroll-padding-top:env(safe-area-inset-top,0px)}
body{font-family:var(--body);background:var(--bg);color:var(--fg);line-height:1.6;-webkit-font-smoothing:antialiased;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--bg);z-index:20}
a{color:var(--accent);text-decoration:none}a:hover{text-decoration:underline}
.w{max-width:1060px;margin:0 auto;padding:0 28px}
nav{position:sticky;top:env(safe-area-inset-top,0px);z-index:15;background:var(--bg);border-bottom:1px solid var(--border);padding:14px 0}
nav .w{display:flex;justify-content:space-between;align-items:center}
.nn{font-family:var(--display);font-weight:700;font-size:1rem;letter-spacing:-.02em;color:var(--fg)}
.nl{display:flex;gap:24px}.nl a{font-family:var(--display);font-size:.82rem;font-weight:500;color:var(--fg-mid)}.nl a:hover{color:var(--fg);text-decoration:none}
.hero{padding:100px 0 90px;border-bottom:1px solid var(--border)}
.ht{display:inline-block;font-family:var(--display);font-size:.78rem;font-weight:600;color:var(--accent);background:var(--accent-glow);padding:6px 14px;border-radius:4px;margin-bottom:28px}
.hero h1{font-family:var(--display);font-size:clamp(2.8rem,6vw,4.2rem);font-weight:700;line-height:1.08;letter-spacing:-.035em;max-width:750px;margin-bottom:28px}
.hero h1 em{font-family:var(--body);font-style:italic;font-weight:400}
.hs{font-size:1.15rem;color:var(--fg-mid);max-width:560px;line-height:1.65;margin-bottom:40px}
.hc{display:flex;gap:28px;flex-wrap:wrap}.hc a{font-family:var(--display);font-size:.84rem;font-weight:500;color:var(--fg-dim);transition:color .2s}.hc a:hover{color:var(--fg);text-decoration:none}
section{padding:80px 0}section+section{border-top:1px solid var(--border)}
.sh{margin-bottom:56px}.sl{font-family:var(--display);font-size:.72rem;font-weight:600;color:var(--fg-dim);letter-spacing:.08em;text-transform:uppercase;margin-bottom:10px}
.st{font-family:var(--display);font-size:clamp(1.8rem,3.5vw,2.5rem);font-weight:700;letter-spacing:-.03em;line-height:1.15}
.pb{display:grid;grid-template-columns:1fr 1fr;gap:0;border:1px solid var(--border);border-radius:10px;overflow:hidden;margin-bottom:28px;background:var(--bg-card)}
.pc{padding:40px;display:flex;flex-direction:column}.pe{background:var(--bg-ev);padding:40px;display:flex;flex-direction:column;gap:16px;border-left:1px solid var(--border)}
.pt{font-family:var(--display);font-size:.72rem;font-weight:600;color:var(--accent);margin-bottom:8px}
.pn{font-family:var(--display);font-size:1.55rem;font-weight:700;letter-spacing:-.02em;margin-bottom:14px;line-height:1.2}
.pd{font-size:1rem;color:var(--fg-mid);line-height:1.65;flex-grow:1}
.pl{margin-top:20px;font-family:var(--display);font-size:.84rem;font-weight:600}
.el{font-family:var(--display);font-size:.68rem;font-weight:600;color:var(--fg-dim);letter-spacing:.06em;text-transform:uppercase;margin-bottom:12px}
.mr{display:flex;justify-content:space-between;align-items:baseline;padding:12px 0;border-bottom:1px solid var(--border)}.mr:last-child{border-bottom:none}
.ml{font-family:var(--display);font-size:.82rem;color:var(--fg-mid)}.mv{font-family:var(--display);font-size:.88rem;font-weight:700;color:var(--fg)}
.mv.h{color:var(--accent)}.mv.g{color:var(--green)}
.bn{text-align:center;padding:24px 0}.bn .n{font-family:var(--display);font-size:3rem;font-weight:700;letter-spacing:-.04em;line-height:1;color:var(--accent)}
.bn .nl2{font-family:var(--display);font-size:.78rem;color:var(--fg-dim);margin-top:6px}
.ib{background:var(--accent-glow);border-left:3px solid var(--accent);padding:16px 20px;border-radius:0 6px 6px 0;margin-top:auto}
.ib p{font-family:var(--display);font-size:.82rem;color:var(--fg);line-height:1.5}
.ib.gb{background:var(--green-dim);border-left-color:var(--green)}
.sy{font-family:var(--display);font-size:.88rem;font-weight:600;color:var(--fg-mid);margin-bottom:20px;margin-top:20px}
.sg{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
.sc{background:var(--bg-card);border:1px solid var(--border);border-radius:8px;padding:24px;transition:border-color .2s;text-decoration:none;color:inherit;display:block}
.sc:hover{border-color:var(--fg-dim);text-decoration:none}
.sc h4{font-family:var(--display);font-size:1.05rem;font-weight:700;margin-bottom:8px;letter-spacing:-.01em;color:var(--fg)}
.sc p{font-size:.88rem;color:var(--fg-mid);line-height:1.5}
.ar{display:grid;grid-template-columns:repeat(3,1fr);gap:20px}
.ai{background:var(--bg-card);border:1px solid var(--border);border-radius:8px;padding:32px 28px}
.an{font-family:var(--display);font-size:3.5rem;font-weight:700;color:var(--border);line-height:1;margin-bottom:16px}
.ai h3{font-family:var(--display);font-size:1rem;font-weight:700;margin-bottom:10px}.ai p{font-size:.9rem;color:var(--fg-mid);line-height:1.55}
.eb{display:grid;grid-template-columns:180px 1fr;gap:28px;padding:28px 0;border-bottom:1px solid var(--border)}.eb:last-child{border-bottom:none}
.ew{font-family:var(--display);font-size:.82rem;color:var(--fg-dim);padding-top:4px}
.ex h3{font-family:var(--display);font-size:1.05rem;font-weight:700;margin-bottom:2px}
.ex .er{font-size:.9rem;color:var(--fg-mid);font-style:italic;margin-bottom:10px}
.ex p{font-size:.92rem;color:var(--fg-mid);line-height:1.6}
footer{border-top:1px solid var(--border);padding:48px 0 60px}
.fr{display:flex;justify-content:space-between;align-items:flex-start;flex-wrap:wrap;gap:20px}
.fr p{font-size:.85rem;color:var(--fg-dim);margin-top:4px}
.fl{display:flex;gap:24px}.fl a{font-family:var(--display);font-size:.84rem;font-weight:500;color:var(--fg-mid)}
@media(max-width:740px){.pb{grid-template-columns:1fr}.pe{border-left:none;border-top:1px solid var(--border)}.ar,.sg{grid-template-columns:1fr}.eb{grid-template-columns:1fr;gap:4px}.hero{padding:60px 0 50px}section{padding:50px 0}.pc,.pe{padding:28px}}
</style>
</head>
<body>
<nav><div class="w"><span class="nn">Udeesha Bansal</span><div class="nl"><a href="#work">Work</a><a href="#approach">Approach</a><a href="#experience">Experience</a><a href="mailto:udeesha.v.bansal@gmail.com">Contact</a></div></div></nav>

<header class="hero"><div class="w">
<div class="ht">Open to strategy, consulting & analytical roles</div>
<h1>Research the problem. Build the framework. <em>Deliver the answer.</em></h1>
<p class="hs">I work across market entry strategy, commercial due diligence, operational transformation and AI-powered analytics. From 418-company screens to system implementations, I do the work that turns ambiguity into decisions.</p>
<div class="hc"><a href="mailto:udeesha.v.bansal@gmail.com">udeesha.v.bansal@gmail.com</a><a href="tel:+6585356368">+65 8535 6368</a><a href="https://www.linkedin.com/in/udeesha-bansal-4a01b01b4/" target="_blank">LinkedIn</a><a href="https://github.com/udeeshabansal" target="_blank">GitHub</a></div>
</div></header>

<section id="work"><div class="w">
<div class="sh"><div class="sl">Selected work</div><h2 class="st">Four problems, four frameworks</h2></div>

<div class="pb"><div class="pc">
<div class="pt">Market Entry Strategy & Commercial Due Diligence</div>
<h3 class="pn">Project Causeway</h3>
<p class="pd">A Japanese M&E corporation wanted to enter data-centre services in Singapore and Malaysia. I mapped regulatory constraints and licensing barriers in both markets, screened 418 contractors through four filters, and challenged the board's assumption that the largest target is the best. Recommended a two-country acquisition platform structured around ownership caps and regulatory logic.</p>
</div><div class="pe">
<div class="el">The evidence</div>
<div class="bn"><div class="n">418</div><div class="nl2">contractors screened across two markets</div></div>
<div class="mr"><span class="ml">Targets shortlisted</span><span class="mv">4 of 418</span></div>
<div class="mr"><span class="ml">Malaysia stake</span><span class="mv">30% minority</span></div>
<div class="mr"><span class="ml">Singapore stake</span><span class="mv">65% control</span></div>
<div class="mr"><span class="ml">Deal size</span><span class="mv h">US$68-99M</span></div>
<div class="ib"><p>The board's "largest target" rule would have selected the weakest candidate. The screening proved it.</p></div>
</div></div>

<div class="pb"><div class="pc">
<div class="pt">AI-Powered Strategic Analytics</div>
<h3 class="pn">The Quiet Signal Engine</h3>
<p class="pd">Built an NLP tool that tracks how management language shifts across earnings calls, surfacing changes in confidence, strategic priorities and guidance framing that conventional analysis misses. Four independent detectors run per metric per quarter. A convergence engine finds where multiple channels agree.</p>
<a class="pl" href="https://github.com/udeeshabansal/earnings-signal-engine" target="_blank">View code and research memo &rarr;</a>
</div><div class="pe">
<div class="el">Backtested across 13 quarters of Novo Nordisk</div>
<div class="bn"><div class="n" style="color:var(--green)">1-2 Qs</div><div class="nl2">early warning before every guidance revision</div></div>
<div class="mr"><span class="ml">Quarters analysed</span><span class="mv">13</span></div>
<div class="mr"><span class="ml">Detectors</span><span class="mv">4 independent channels</span></div>
<div class="mr"><span class="ml">Stock from high</span><span class="mv h">-31%</span></div>
<div class="mr"><span class="ml">Consensus</span><span class="mv">Hold</span></div>
<div class="ib gb"><p>The board replaced the CEO citing decline "since mid-2024." The engine's strongest signal fired eleven months earlier.</p></div>
</div></div>

<div class="pb"><div class="pc">
<div class="pt">Strategy Development & Operational Transformation</div>
<h3 class="pn">Tsao Family Foundation</h3>
<p class="pd">Two parallel workstreams at a philanthropic foundation. First: developed a humanitarian funding strategy that shifted the organisation from reactive disaster response to a planned approach with a structured shortlist. Recommendations advanced to the management committee. Second: leading a CRM and grant management system implementation end-to-end.</p>
</div><div class="pe">
<div class="el">Strategy workstream</div>
<div class="mr"><span class="ml">Countries researched</span><span class="mv">27</span></div>
<div class="mr"><span class="ml">Organisations screened</span><span class="mv">61</span></div>
<div class="mr"><span class="ml">Priority pillars</span><span class="mv">8</span></div>
<div class="mr"><span class="ml">Outcome</span><span class="mv g">Advanced to mgmt committee</span></div>
<div class="el" style="margin-top:20px">Transformation workstream</div>
<div class="mr"><span class="ml">Process stages mapped</span><span class="mv">7</span></div>
<div class="mr"><span class="ml">Users onboarded</span><span class="mv">6 across 3 tiers</span></div>
<div class="mr"><span class="ml">Status</span><span class="mv">In progress</span></div>
</div></div>

<div class="pb"><div class="pc">
<div class="pt">Strategic Growth Assessment</div>
<h3 class="pn">Seatrium Expansion</h3>
<p class="pd">Seatrium (SGX-listed offshore and marine) needed to move beyond project-based revenue. Evaluated strategic expansion options and recommended a partnership-first entry into offshore wind lifecycle services via IWS (Oslo) with an option on control, structured around operational fit and commercial logic.</p>
</div><div class="pe">
<div class="el">The recommendation</div>
<div class="mr"><span class="ml">Client</span><span class="mv">Seatrium (SGX)</span></div>
<div class="mr"><span class="ml">Target</span><span class="mv">IWS, Oslo</span></div>
<div class="mr"><span class="ml">Entry model</span><span class="mv g">Partnership-first</span></div>
<div class="mr"><span class="ml">Optionality</span><span class="mv">Option on control</span></div>
<div class="ib"><p>Structured around lifecycle service capabilities and commercial fit, not financial engineering.</p></div>
</div></div>

<div class="sy">Financial analysis and interactive models</div>
<div class="sg">
<a href="https://sbux-simulator.vercel.app/" target="_blank" class="sc"><div class="pt">Valuation</div><h4>Starbucks</h4><p>DCF with 10,000 Monte Carlo simulations. Interactive scenario explorer.</p></a>
<div class="sc"><div class="pt">Supply Chain & FX Risk</div><h4>On Holding</h4><p>Tariff and FX exposure modelling with supply-chain alternatives and margin scenarios.</p></div>
<div class="sc"><div class="pt">Market Entry & Fintech</div><h4>HALA Holding</h4><p>TAM sizing, competitive moat, revenue model and exit thesis for a Saudi fintech.</p></div>
<div class="sc"><div class="pt">Financial Health</div><h4>CVS Health</h4><p>Piotrowski F-Score diagnostic, peer benchmarking and margin decomposition.</p></div>
<div class="sc"><div class="pt">Corporate Finance</div><h4>Pfizer</h4><p>Integrated 3-statement model, DCF, DuPont analysis and scenario modelling.</p></div>
<div class="sc"><div class="pt">Corporate Finance</div><h4>Reliance Industries</h4><p>Segment-level revenue modelling, DCF valuation and sensitivity analysis.</p></div>
</div>
</div></section>

<section id="approach"><div class="w">
<div class="sh"><div class="sl">How I work</div><h2 class="st">Beyond the model</h2></div>
<div class="ar">
<div class="ai"><div class="an">1</div><h3>Find the real question</h3><p>Identify the decision, the constraints, and which evidence actually matters. Most problems arrive framed too broadly or too narrowly.</p></div>
<div class="ai"><div class="an">2</div><h3>Stress-test the story</h3><p>Build scenarios and distinguish strong evidence from uncertain assumptions. The goal is to know where the thesis breaks, not to prove it.</p></div>
<div class="ai"><div class="an">3</div><h3>Make it useful</h3><p>Deliver a recommendation, model, process or system others can act on. Analysis that stays in a spreadsheet is unfinished work.</p></div>
</div>
</div></section>

<section id="experience"><div class="w">
<div class="sh"><div class="sl">Experience & education</div><h2 class="st">Where I have worked</h2></div>
<div class="eb"><div class="ew">Aug 2026 - Present</div><div class="ex"><h3>Tsao Family Foundation, Singapore</h3><div class="er">Finance & Operations Intern</div><p>Developed a humanitarian funding strategy across 27 countries and 61 organisations. Leading a CRM and grant management system implementation end-to-end. Built scenario-based impact tools for resource prioritisation. Recommendations advanced to the management committee.</p></div></div>
<div class="eb"><div class="ew">Aug 2023 - Jan 2024</div><div class="ex"><h3>Agarwal Manoj Nidhi & Associates, Delhi</h3><div class="er">Audit Intern</div><p>Evaluated business processes and internal controls across five client engagements, identifying risk areas and documenting findings for management review.</p></div></div>
<div class="eb"><div class="ew">Apr 2022 - Mar 2023</div><div class="ex"><h3>ACHS & Co., Delhi</h3><div class="er">Taxation & Compliance Intern</div><p>Managed concurrent compliance delivery for 20+ corporate clients, coordinating cross-functional information flows to meet regulatory deadlines.</p></div></div>
<div class="eb" style="border-bottom:1px solid var(--border)"><div class="ew">Aug 2025 - Nov 2026</div><div class="ex"><h3>Singapore Management University</h3><div class="er">MSc Management (Finance specialisation)</div><p>Recipient, Impact on Asia Scholarship</p></div></div>
<div class="eb"><div class="ew">Jul 2022 - Jul 2025</div><div class="ex"><h3>Indira Gandhi National Open University</h3><div class="er">Bachelor of Commerce</div></div></div>
</div></section>

<footer><div class="w"><div class="fr"><div><span class="nn">Udeesha Bansal</span><p>Exploring opportunities across strategy, consulting, analytics and transformation.</p></div><div class="fl"><a href="mailto:udeesha.v.bansal@gmail.com">Email</a><a href="https://www.linkedin.com/in/udeesha-bansal-4a01b01b4/" target="_blank">LinkedIn</a><a href="https://github.com/udeeshabansal" target="_blank">GitHub</a></div></div></div></footer>
</body></html>
