<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Udeesha Bansal | Strategy · Analytics · Decisions</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
:root{
  --bg:#0d1117;--card:#161b22;--card-border:#21262d;
  --fg:#e6edf3;--fg-mid:#8b949e;--fg-dim:#484f58;
  --accent:#c9a84c;--accent-glow:rgba(201,168,76,.12);
  --teal:#58a6b0;--teal-glow:rgba(88,166,176,.1);
  --sans:'Inter',system-ui,sans-serif;
  --display:'Playfair Display',Georgia,serif;
}
html{scroll-behavior:smooth}
body{font-family:var(--sans);background:var(--bg);color:var(--fg);line-height:1.6;-webkit-font-smoothing:antialiased}
a{color:var(--accent);text-decoration:none}a:hover{text-decoration:underline}

/* ── HERO ── */
.hero{text-align:center;padding:80px 24px 60px;max-width:720px;margin:0 auto}
.hero-avatar{width:120px;height:120px;border-radius:50%;background:linear-gradient(135deg,var(--accent),var(--teal));margin:0 auto 24px;display:flex;align-items:center;justify-content:center;font-family:var(--display);font-size:2.4rem;color:var(--bg);font-weight:700}
.hero-hello{font-size:.9rem;color:var(--fg-mid);margin-bottom:8px}
.hero h1{font-family:var(--display);font-size:clamp(2.4rem,5vw,3.4rem);font-weight:700;letter-spacing:-.02em;margin-bottom:12px}
.hero-sub{font-size:1.1rem;color:var(--accent);font-weight:600;margin-bottom:20px}
.hero-desc{font-size:1rem;color:var(--fg-mid);max-width:560px;margin:0 auto 32px;line-height:1.7}
.hero-btns{display:flex;gap:14px;justify-content:center;margin-bottom:28px;flex-wrap:wrap}
.btn-primary{background:var(--accent);color:var(--bg);padding:12px 28px;border-radius:8px;font-weight:600;font-size:.9rem;transition:opacity .2s}
.btn-primary:hover{opacity:.85;text-decoration:none}
.btn-outline{border:1px solid var(--card-border);color:var(--fg);padding:12px 28px;border-radius:8px;font-weight:600;font-size:.9rem;transition:border-color .2s}
.btn-outline:hover{border-color:var(--fg-mid);text-decoration:none}
.hero-social{display:flex;gap:16px;justify-content:center}
.hero-social a{width:40px;height:40px;border-radius:50%;border:1px solid var(--card-border);display:flex;align-items:center;justify-content:center;color:var(--fg-mid);font-size:.8rem;transition:border-color .2s,color .2s}
.hero-social a:hover{border-color:var(--accent);color:var(--accent);text-decoration:none}

/* ── STATS ── */
.stats{display:flex;gap:16px;justify-content:center;padding:0 24px 60px;max-width:640px;margin:0 auto}
.stat{flex:1;background:var(--card);border:1px solid var(--card-border);border-radius:12px;padding:24px 16px;text-align:center}
.stat-num{font-size:2rem;font-weight:700;color:var(--teal);letter-spacing:-.03em}
.stat-label{font-size:.75rem;color:var(--fg-dim);text-transform:uppercase;letter-spacing:.08em;margin-top:4px}

/* ── SECTIONS ── */
section{padding:60px 24px;max-width:960px;margin:0 auto}
.sec-tag{text-align:center;margin-bottom:12px}
.sec-tag span{font-size:.72rem;font-weight:600;color:var(--accent);background:var(--accent-glow);padding:6px 16px;border-radius:20px;text-transform:uppercase;letter-spacing:.08em}
.sec-title{font-family:var(--display);font-size:clamp(1.8rem,3.5vw,2.4rem);font-weight:700;text-align:center;margin-bottom:12px}
.sec-sub{text-align:center;color:var(--fg-mid);font-size:.95rem;margin-bottom:48px}

/* ── ABOUT ── */
.about-grid{display:grid;grid-template-columns:1.4fr 1fr;gap:20px}
.about-bio{background:var(--card);border:1px solid var(--card-border);border-radius:12px;padding:36px;font-size:.95rem;color:var(--fg-mid);line-height:1.75}
.about-facts{background:var(--card);border:1px solid var(--card-border);border-radius:12px;padding:36px}
.about-facts h3{font-size:1rem;font-weight:700;margin-bottom:20px}
.fact{display:flex;align-items:flex-start;gap:12px;margin-bottom:16px}
.fact-icon{width:36px;height:36px;border-radius:8px;background:var(--teal-glow);border:1px solid rgba(88,166,176,.2);display:flex;align-items:center;justify-content:center;font-size:.85rem;flex-shrink:0;color:var(--teal)}
.fact-text .fl{font-size:.75rem;color:var(--fg-dim)}.fact-text .fv{font-size:.88rem;font-weight:500}

/* ── SKILLS GRID ── */
.skills-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.skill-card{background:var(--card);border:1px solid var(--card-border);border-radius:12px;padding:32px}
.skill-card h3{font-size:1.05rem;font-weight:700;margin-bottom:8px}
.skill-card p{font-size:.88rem;color:var(--fg-mid);line-height:1.6;margin-bottom:16px}
.pills{display:flex;flex-wrap:wrap;gap:8px}
.pill{font-size:.78rem;padding:6px 14px;border-radius:20px;border:1px solid var(--card-border);color:var(--fg-mid);background:transparent;transition:border-color .2s,color .2s}
.pill.hl{border-color:var(--accent);color:var(--accent)}

/* ── PROJECTS ── */
.project{background:var(--card);border:1px solid var(--card-border);border-radius:12px;padding:36px;margin-bottom:20px}
.project-tag{font-size:.72rem;font-weight:600;color:var(--teal);text-transform:uppercase;letter-spacing:.06em;margin-bottom:8px}
.project h3{font-size:1.3rem;font-weight:700;margin-bottom:12px}
.project p{font-size:.92rem;color:var(--fg-mid);line-height:1.7;margin-bottom:16px}
.project-metrics{display:flex;gap:24px;flex-wrap:wrap;margin-bottom:16px}
.pm{display:flex;flex-direction:column}
.pm-val{font-size:1.1rem;font-weight:700;color:var(--accent)}
.pm-label{font-size:.72rem;color:var(--fg-dim);text-transform:uppercase;letter-spacing:.06em}
.project-insight{background:var(--accent-glow);border-left:3px solid var(--accent);padding:14px 18px;border-radius:0 8px 8px 0;margin-top:8px}
.project-insight p{color:var(--fg);font-size:.85rem;margin:0;font-weight:500}
.project a.pl{font-size:.85rem;font-weight:600;display:inline-block;margin-top:12px}

/* ── EXPERIENCE ── */
.exp{border-left:2px solid var(--card-border);margin-left:20px;padding-left:32px;position:relative;padding-bottom:36px}
.exp:last-child{padding-bottom:0}
.exp::before{content:'';position:absolute;left:-7px;top:4px;width:12px;height:12px;border-radius:50%;background:var(--accent);border:2px solid var(--bg)}
.exp-when{font-size:.8rem;color:var(--fg-dim);margin-bottom:4px}
.exp h3{font-size:1rem;font-weight:700;margin-bottom:2px}
.exp-role{font-size:.88rem;color:var(--teal);font-weight:500;margin-bottom:8px}
.exp p{font-size:.88rem;color:var(--fg-mid);line-height:1.6}

/* ── EDUCATION ── */
.edu-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.edu{background:var(--card);border:1px solid var(--card-border);border-radius:12px;padding:28px}
.edu h3{font-size:1rem;font-weight:700;margin-bottom:4px}
.edu-deg{font-size:.88rem;color:var(--teal);margin-bottom:4px}
.edu-when{font-size:.8rem;color:var(--fg-dim)}

/* ── FOOTER ── */
footer{text-align:center;padding:60px 24px 40px;border-top:1px solid var(--card-border);margin-top:40px}
footer h2{font-family:var(--display);font-size:1.6rem;margin-bottom:8px}
footer p{color:var(--fg-mid);font-size:.9rem;margin-bottom:24px}
.foot-links{display:flex;gap:20px;justify-content:center;flex-wrap:wrap}
.foot-links a{font-size:.85rem;font-weight:500;color:var(--fg-mid)}
.foot-copy{margin-top:40px;font-size:.75rem;color:var(--fg-dim)}

@media(max-width:700px){
  .about-grid,.skills-grid,.edu-grid{grid-template-columns:1fr}
  .stats{flex-direction:row;gap:10px}
  .stat{padding:16px 10px}
  .project-metrics{gap:16px}
  .hero{padding:50px 20px 40px}
  section{padding:40px 20px}
}
</style>
</head>
<body>

<header class="hero">
  <div class="hero-avatar">UB</div>
  <div class="hero-hello">Hello, I'm</div>
  <h1>Udeesha Bansal</h1>
  <div class="hero-sub">Strategy & Operations | SMU Singapore</div>
  <p class="hero-desc">I work across market entry strategy, commercial due diligence, operational transformation and AI-powered analytics. From 418-company screens to system implementations, I turn ambiguity into decisions leadership can act on.</p>
  <div class="hero-btns">
    <a href="mailto:udeesha.v.bansal@gmail.com" class="btn-primary">Get In Touch</a>
    <a href="#projects" class="btn-outline">View My Work</a>
  </div>
  <div class="hero-social">
    <a href="mailto:udeesha.v.bansal@gmail.com" title="Email">@</a>
    <a href="https://www.linkedin.com/in/udeesha-bansal-4a01b01b4/" target="_blank" title="LinkedIn">in</a>
    <a href="https://github.com/udeeshabansal" target="_blank" title="GitHub">GH</a>
  </div>
</header>

<div class="stats">
  <div class="stat"><div class="stat-num">4</div><div class="stat-label">Strategy Projects</div></div>
  <div class="stat"><div class="stat-num">418</div><div class="stat-label">Targets Screened</div></div>
  <div class="stat"><div class="stat-num">27</div><div class="stat-label">Countries Researched</div></div>
</div>

<!-- ABOUT -->
<section id="about">
  <div class="sec-tag"><span>About Me</span></div>
  <h2 class="sec-title">About Me</h2>
  <div class="sec-sub">Background, approach and what I care about.</div>
  <div class="about-grid">
    <div class="about-bio">
      I'm an MSc Management (Finance) candidate at Singapore Management University, working as a Finance & Operations Intern at the Tsao Family Foundation. My work sits at the intersection of strategy and execution: I've built a humanitarian funding strategy from scratch across 27 countries, led a CRM and grant management system implementation, and independently produced a commercial due diligence case that screened 418 contractors to recommend a staged market entry. I also build tools — an NLP engine that reads earnings-call language to detect strategic shifts before they hit the numbers. I'm drawn to problems where the question isn't clear yet, and where the answer has to be something someone can actually use.
    </div>
    <div class="about-facts">
      <h3>Quick Facts</h3>
      <div class="fact">
        <div class="fact-icon">@</div>
        <div class="fact-text"><div class="fl">Email</div><div class="fv">udeesha.v.bansal@gmail.com</div></div>
      </div>
      <div class="fact">
        <div class="fact-icon">+</div>
        <div class="fact-text"><div class="fl">Phone</div><div class="fv">+65 8535 6368</div></div>
      </div>
      <div class="fact">
        <div class="fact-icon">◎</div>
        <div class="fact-text"><div class="fl">Location</div><div class="fv">Singapore</div></div>
      </div>
      <div class="fact">
        <div class="fact-icon">↗</div>
        <div class="fact-text"><div class="fl">Status</div><div class="fv">Open to opportunities</div></div>
      </div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="sec-tag"><span>Skills & Tools</span></div>
  <h2 class="sec-title">Skills & Tools</h2>
  <div class="sec-sub">The strengths and tools I bring to my work.</div>
  <div class="skills-grid">
    <div class="skill-card">
      <h3>Problem Types</h3>
      <p>The kinds of work I keep coming back to, where research meets structured decision-making.</p>
      <div class="pills">
        <span class="pill">Market Entry Strategy</span>
        <span class="pill hl">Commercial Due Diligence</span>
        <span class="pill">Operational Transformation</span>
        <span class="pill">System Implementation</span>
        <span class="pill">Humanitarian Strategy</span>
      </div>
    </div>
    <div class="skill-card">
      <h3>Frameworks I Use</h3>
      <p>Not borrowed methodology breadth, but the tools that show up in nearly every project I work on.</p>
      <div class="pills">
        <span class="pill hl">Scenario Planning</span>
        <span class="pill">Sensitivity Analysis</span>
        <span class="pill">Stakeholder Mapping</span>
        <span class="pill">Process Redesign</span>
        <span class="pill">NLP Signal Detection</span>
      </div>
    </div>
    <div class="skill-card">
      <h3>Industries</h3>
      <p>Sectors where my project work reflects real depth, not surface-level exposure.</p>
      <div class="pills">
        <span class="pill">Philanthropy & Impact</span>
        <span class="pill hl">Data Centres & M&E</span>
        <span class="pill">Offshore & Marine</span>
        <span class="pill">Healthcare & Pharma</span>
        <span class="pill">Fintech</span>
      </div>
    </div>
    <div class="skill-card">
      <h3>How I Work</h3>
      <p>The operating practices that turn a four-week project into a clear recommendation.</p>
      <div class="pills">
        <span class="pill">Structured Screening</span>
        <span class="pill hl">Slide-Driven Synthesis</span>
        <span class="pill">Quantitative Analysis (SQL, Excel)</span>
        <span class="pill">Vendor Coordination</span>
        <span class="pill">Training Design</span>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="sec-tag"><span>Selected Work</span></div>
  <h2 class="sec-title">Projects</h2>
  <div class="sec-sub">Four problems, four frameworks, four answers.</div>

  <div class="project">
    <div class="project-tag">Market Entry Strategy & Commercial Due Diligence</div>
    <h3>Project Causeway</h3>
    <p>A Japanese M&E corporation wanted to enter data-centre services in Singapore and Malaysia. I mapped regulatory constraints and licensing barriers in both markets, screened 418 contractors through four filters, and challenged the board's assumption that the largest target is the best. Recommended a two-country acquisition platform structured around ownership caps and regulatory logic.</p>
    <div class="project-metrics">
      <div class="pm"><span class="pm-val">418</span><span class="pm-label">Targets screened</span></div>
      <div class="pm"><span class="pm-val">4</span><span class="pm-label">Shortlisted</span></div>
      <div class="pm"><span class="pm-val">US$68-99M</span><span class="pm-label">Deal size</span></div>
      <div class="pm"><span class="pm-val">2</span><span class="pm-label">Countries</span></div>
    </div>
    <div class="project-insight"><p>The board's "largest target" rule would have selected the weakest candidate. The screening proved it.</p></div>
  </div>

  <div class="project">
    <div class="project-tag">AI-Powered Strategic Analytics</div>
    <h3>The Quiet Signal Engine</h3>
    <p>Built an NLP tool that tracks how management language shifts across earnings calls, surfacing changes in confidence, strategic priorities and guidance framing that conventional analysis misses. Four independent detectors run per metric per quarter. A convergence engine finds where multiple channels agree.</p>
    <div class="project-metrics">
      <div class="pm"><span class="pm-val">13</span><span class="pm-label">Quarters analysed</span></div>
      <div class="pm"><span class="pm-val">4</span><span class="pm-label">Detector channels</span></div>
      <div class="pm"><span class="pm-val">1-2 Qs</span><span class="pm-label">Early warning</span></div>
      <div class="pm"><span class="pm-val">-31%</span><span class="pm-label">Stock from high</span></div>
    </div>
    <div class="project-insight"><p>The board replaced the CEO citing decline "since mid-2024." The engine's strongest signal fired eleven months earlier, reading nothing but transcripts.</p></div>
    <a class="pl" href="https://github.com/udeeshabansal/earnings-signal-engine" target="_blank">View code and research memo &rarr;</a>
  </div>

  <div class="project">
    <div class="project-tag">Strategy Development & Operational Transformation</div>
    <h3>Tsao Family Foundation</h3>
    <p>Two parallel workstreams at a philanthropic foundation. First: developed a humanitarian funding strategy by researching 27 countries and screening 61 organisations against eight priority pillars, shifting the foundation from reactive disaster response to a planned approach. Recommendations advanced to the management committee. Second: leading a CRM and grant management system implementation end-to-end.</p>
    <div class="project-metrics">
      <div class="pm"><span class="pm-val">27</span><span class="pm-label">Countries</span></div>
      <div class="pm"><span class="pm-val">61</span><span class="pm-label">Organisations</span></div>
      <div class="pm"><span class="pm-val">7</span><span class="pm-label">Process stages mapped</span></div>
      <div class="pm"><span class="pm-val">6</span><span class="pm-label">Users onboarded</span></div>
    </div>
  </div>

  <div class="project">
    <div class="project-tag">Strategic Growth Assessment</div>
    <h3>Seatrium Expansion</h3>
    <p>Seatrium (SGX-listed offshore and marine) needed to move beyond project-based revenue. Evaluated strategic expansion options and recommended a partnership-first entry into offshore wind lifecycle services via IWS (Oslo) with an option on control, structured around operational fit and commercial logic.</p>
    <div class="project-metrics">
      <div class="pm"><span class="pm-val">Seatrium</span><span class="pm-label">Client (SGX)</span></div>
      <div class="pm"><span class="pm-val">IWS Oslo</span><span class="pm-label">Target</span></div>
      <div class="pm"><span class="pm-val">Partnership</span><span class="pm-label">Entry model</span></div>
    </div>
    <div class="project-insight"><p>Structured around lifecycle service capabilities and commercial fit, not financial engineering.</p></div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="sec-tag"><span>Experience</span></div>
  <h2 class="sec-title">Experience</h2>
  <div class="sec-sub">Hands-on work across strategy, transformation, audit and compliance.</div>

  <div class="exp">
    <div class="exp-when">Aug 2026 - Present</div>
    <h3>Tsao Family Foundation, Singapore</h3>
    <div class="exp-role">Finance & Operations Intern</div>
    <p>Developed a humanitarian funding strategy across 27 countries and 61 organisations. Leading a CRM and grant management system implementation end-to-end. Conducted rapid due diligence on three organisations for emergency flood-response funding. Recommendations advanced to the management committee.</p>
  </div>

  <div class="exp">
    <div class="exp-when">Aug 2023 - Jan 2024</div>
    <h3>Agarwal Manoj Nidhi & Associates, Delhi</h3>
    <div class="exp-role">Audit Intern</div>
    <p>Evaluated business processes and internal controls across five client engagements, identifying risk areas and documenting findings for management review.</p>
  </div>

  <div class="exp">
    <div class="exp-when">Apr 2022 - Mar 2023</div>
    <h3>ACHS & Co., Delhi</h3>
    <div class="exp-role">Taxation & Compliance Intern</div>
    <p>Managed concurrent compliance delivery for 20+ corporate clients, coordinating cross-functional information flows to meet regulatory deadlines.</p>
  </div>
</section>

<!-- EDUCATION -->
<section id="education">
  <div class="sec-tag"><span>Education</span></div>
  <h2 class="sec-title">Education</h2>
  <div class="sec-sub"></div>
  <div class="edu-grid">
    <div class="edu">
      <h3>Singapore Management University</h3>
      <div class="edu-deg">MSc Management (Finance specialisation)</div>
      <div class="edu-when">Aug 2025 - Nov 2026 | Impact on Asia Scholarship</div>
    </div>
    <div class="edu">
      <h3>Indira Gandhi National Open University</h3>
      <div class="edu-deg">Bachelor of Commerce</div>
      <div class="edu-when">Jul 2022 - Jul 2025</div>
    </div>
  </div>
</section>

<footer>
  <h2>Let's talk.</h2>
  <p>Exploring opportunities across strategy, consulting, analytics and transformation.</p>
  <div class="foot-links">
    <a href="mailto:udeesha.v.bansal@gmail.com">udeesha.v.bansal@gmail.com</a>
    <a href="tel:+6585356368">+65 8535 6368</a>
    <a href="https://www.linkedin.com/in/udeesha-bansal-4a01b01b4/" target="_blank">LinkedIn</a>
    <a href="https://github.com/udeeshabansal" target="_blank">GitHub</a>
  </div>
  <div class="foot-copy">&copy; 2026 Udeesha Bansal</div>
</footer>

</body>
</html>
