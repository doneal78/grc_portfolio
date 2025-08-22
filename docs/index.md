---
layout: default
title: Home
---

<header class="hero">
  <div class="hero__inner">
    <h1>GRC + Security Engineering Portfolio</h1>
    <p class="lead">Governance that scales, risk programs tied to business impact, and audit-ready artifacts.</p>
    <div class="cta-row">
      <!-- Scrolls to Projects on this page -->
      <a class="btn btn-primary" href="{{ '/#projects' | relative_url }}">See Projects</a>
      <!-- Opens Templates page -->
      <a class="btn btn-ghost" href="{{ '/portfolio-templates/' | relative_url }}">Templates & Resources</a>
    </div>
  </div>
</header>

<section id="highlights" class="section">
  <h2>Highlights</h2>
  <div class="card-grid">
    <a class="card" href="{{ '/labs/aws-account-governance/' | relative_url }}">
      <h3>AWS Governance Lab</h3>
      <p>Identity Center, Config, Security Hub, Budgets—controls with screenshots & triage.</p>
      <span class="pill">Hands-on</span>
    </a>

    <a class="card" href="{{ '/projects/risk-assessment/' | relative_url }}">
      <h3>Risk Assessment (Simulated)</h3>
      <p>Risk register, FAIR-lite scoring, treatment plan, and exec summary.</p>
      <span class="pill">Methodology</span>
    </a>

    <a class="card" href="{{ '/projects/aws-account-governance/' | relative_url }}">
      <h3>AWS Account Governance</h3>
      <p>Guardrails & least-privilege mapped to NIST CSF with artifacts.</p>
      <span class="pill">Case Study</span>
    </a>
  </div>
</section>

<section id="projects" class="section">
  <h2>Projects</h2>
  <ul class="arrow-list arrow-list--cyan">
    <li><a href="{{ '/projects/aws-account-governance/' | relative_url }}">AWS Account Governance — case study</a></li>
    <li><a href="{{ '/projects/risk-assessment/' | relative_url }}">Enterprise Risk Assessment — register + scoring</a></li>
  </ul>
</section>

<section id="templates" class="section">
  <h2>Templates & Resources</h2>
  <ul class="arrow-list arrow-list--magenta">
    <li><a href="{{ '/portfolio-templates/' | relative_url }}">Portfolio templates (policy, SOP, risk register)</a></li>
    <li><a href="{{ '/resources/' | relative_url }}">Reading list & useful links</a></li>
  </ul>
</section>

<footer class="site-foot">
  <small>© {{ site.time | date: '%Y' }} David O’Neal • <a href="https://www.linkedin.com/in/david-oneal/" target="_blank" rel="noopener">LinkedIn</a></small>
</footer>
