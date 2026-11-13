---
layout: single
title: "Vigie Analytics"
permalink: /
author_profile: false
classes: wide
---

<style>
  /* Hide the default page title + sidebar spacing on the home page */
  .page__title { display: none; }
  .page { width: 100% !important; padding: 0 !important; float: none !important; }

  :root {
    --va-navy: #0f2438;
    --va-teal: #1aa6a6;
    --va-ink: #1d2b36;
    --va-muted: #5b6b78;
    --va-bg: #f5f8fa;
    --va-card: #ffffff;
    --va-line: #e2e9ee;
  }

  .va-wrap { max-width: 1080px; margin: 0 auto; padding: 0 1.25rem; }
  .va-section { padding: 3.5rem 0; }
  .va-section h2 {
    font-size: 1.7rem; color: var(--va-navy); margin: 0 0 .4rem;
    border: none; padding: 0;
  }
  .va-section .va-sub { color: var(--va-muted); margin: 0 0 2rem; }

  /* Hero */
  .va-hero {
    background: linear-gradient(135deg, var(--va-navy) 0%, #17405c 100%);
    color: #fff; padding: 4.5rem 0 4rem;
  }
  .va-hero .va-eyebrow {
    letter-spacing: .14em; text-transform: uppercase; font-size: .8rem;
    color: #7fe0e0; margin: 0 0 .75rem;
  }
  .va-hero h1 { color: #fff; font-size: 2.8rem; margin: 0 0 .75rem; line-height: 1.1; }
  .va-hero p { font-size: 1.15rem; max-width: 620px; color: #d6e3ec; margin: 0 0 1.75rem; }
  .va-btn {
    display: inline-block; padding: .7rem 1.4rem; border-radius: 6px;
    font-weight: 600; text-decoration: none; margin-right: .6rem;
  }
  .va-btn.primary { background: var(--va-teal); color: #fff; }
  .va-btn.ghost { border: 1px solid #7fa3ba; color: #fff; }
  .va-btn:hover { opacity: .9; }

  /* About */
  .va-about { display: grid; grid-template-columns: 220px 1fr; gap: 2.5rem; align-items: center; }
  .va-about img { width: 100%; border-radius: 50%; aspect-ratio: 1/1; object-fit: cover; }
  .va-about p { color: var(--va-ink); line-height: 1.7; margin: 0 0 1rem; }
  .va-meta { color: var(--va-muted); font-size: .95rem; }
  .va-meta a { color: var(--va-teal); }

  /* Skills */
  .va-skills { display: flex; flex-direction: column; gap: 2.5rem; align-items: center; }
  .va-skillrow { display: flex; justify-content: center; flex-wrap: wrap; gap: 2.5rem 3.5rem; width: 100%; }
  .va-skill { width: 130px; text-align: center; transition: transform .15s ease; }
  .va-skill:hover { transform: translateY(-4px); }
  .va-skill img, .va-skill svg { width: 52px; height: 52px; margin: 0 auto .8rem; display: block; color: #3b6fd4; }
  .va-skill .va-mono { width: 52px; height: 52px; margin: 0 auto .8rem; background: var(--va-navy); color: #fff; border-radius: 10px; font-weight: 700; line-height: 52px; }
  .va-skill span { font-weight: 600; color: var(--va-ink); font-size: 1.05rem; }

  /* Projects */
  .va-projects { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1.75rem; }
  .page__content a.va-project {
    display: flex; flex-direction: row; background: #f7f9fa; border: none;
    border-radius: 6px; overflow: hidden; text-decoration: none !important;
    color: inherit !important; box-shadow: none; min-height: 230px;
    transition: transform .15s ease, box-shadow .15s ease;
  }
  .page__content a.va-project:hover { transform: translateY(-3px); box-shadow: 0 8px 22px rgba(15,36,56,.14); }
  .va-project .va-thumb { position: relative; flex: 0 0 38%; background: #dfe7ec; }
  .va-project .va-thumb img { width: 100%; height: 100%; object-fit: cover; display: block; position: absolute; inset: 0; }
  .va-project .va-thumb::after {
    content: "View Project"; position: absolute; inset: 0; display: flex;
    align-items: center; justify-content: center; color: #fff; font-weight: 600;
    background: rgba(15,36,56,.65); opacity: 0; transition: opacity .15s ease;
  }
  .va-project:hover .va-thumb::after { opacity: 1; }
  .va-project .va-body { padding: 1.4rem 1.5rem; flex: 1; }
  .va-project h3 { margin: 0 0 .6rem; font-size: 1.2rem; line-height: 1.25; color: var(--va-navy); text-decoration: none; }
  .va-project p { margin: 0; color: var(--va-muted); font-size: .95rem; line-height: 1.6; text-decoration: none; }
  .va-more { margin-top: 1.75rem; }
  .page__content .va-more a { color: var(--va-teal); font-weight: 600; text-decoration: none; }
  .page__content a.va-btn { text-decoration: none; }
  .page__content a.va-btn.primary, .page__content a.va-btn.ghost { color: #fff; }

  @media (max-width: 720px) {
    .va-hero h1 { font-size: 2.1rem; }
    .va-about { grid-template-columns: 1fr; text-align: center; }
    .va-about img { max-width: 180px; margin: 0 auto; }
    .va-projects { grid-template-columns: 1fr; }
    .va-project { flex-direction: column; }
    .va-project .va-thumb { flex: 0 0 180px; }
  }
</style>

<!-- HERO -->
<header class="va-hero">
  <div class="va-wrap">
    <p class="va-eyebrow">Data analysis · Spatial analytics · Regression modeling</p>
    <h1>Vigie Analytics</h1>
    <p>Turning messy data into clear, defensible answers. I help organizations understand where, why, and how much, using GIS, statistical modeling, and clean visual storytelling.</p>
    <a class="va-btn primary" href="#projects">View projects</a>
    <a class="va-btn ghost" href="mailto:vigieanalytics@gmail.com">Work with me</a>
  </div>
</header>

<!-- ABOUT -->
<section class="va-section" id="about">
  <div class="va-wrap">
    <h2>About Vigie Analytics</h2>
    <p class="va-sub">Founded and led by Gabrielle Dominique</p>
    <div class="va-about">
      <img src="{{ '/images/image.png' | relative_url }}" alt="Gabrielle Dominique">
      <div>
        <p>
          Vigie Analytics is my independent analytics practice. The name comes from the French
          <em>vigie</em>, a lookout: the person watching the horizon so decisions are made with
          the full picture in view.
        </p>
        <p>
          I specialize in spatial analysis, regression modeling, and GIS, taking questions about
          public health, transportation, housing, and consumer markets and turning them into
          analysis that is rigorous, reproducible, and easy to act on.
        </p>
        <p class="va-meta">
          Based in Boston, MA ·
          <a href="mailto:vigieanalytics@gmail.com">Email</a> ·
          <a href="https://www.linkedin.com/in/gabrielle-dominique-786b4123b">LinkedIn</a> ·
          <a href="https://github.com/gabriellejd">GitHub</a> ·
          <a href="{{ '/resume/' | relative_url }}">Resume</a>
        </p>
      </div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section class="va-section va-alt" id="skills">
  <div class="va-wrap">
    <h2>Skills &amp; tools</h2>
    <p class="va-sub">What I use to get from raw data to a finished answer.</p>
    <div class="va-skills">
      <div class="va-skillrow">
        <div class="va-skill">
          <img src="https://cdn.simpleicons.org/r/276DC3" alt="" onerror="this.outerHTML='<div class=&quot;va-mono&quot;>R</div>'">
          <span>R</span>
        </div>
        <div class="va-skill">
          <img src="https://cdn.simpleicons.org/python/3776AB" alt="" onerror="this.outerHTML='<div class=&quot;va-mono&quot;>Py</div>'">
          <span>Python</span>
        </div>
        <div class="va-skill">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><ellipse cx="12" cy="5" rx="8" ry="3"/><path d="M4 5v14c0 1.7 3.6 3 8 3s8-1.3 8-3V5"/><path d="M4 12c0 1.7 3.6 3 8 3s8-1.3 8-3"/></svg>
          <span>SQL</span>
        </div>
        <div class="va-skill">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><circle cx="8" cy="15" r="1" fill="currentColor"/><circle cx="12" cy="11" r="1" fill="currentColor"/><circle cx="16" cy="12" r="1" fill="currentColor"/><circle cx="19" cy="7" r="1" fill="currentColor"/><path d="M6 17L20 6"/></svg>
          <span>Stata</span>
        </div>
        <div class="va-skill">
          <img src="https://cdn.simpleicons.org/cplusplus/00599C" alt="" onerror="this.outerHTML='<div class=&quot;va-mono&quot;>C++</div>'">
          <span>C++</span>
        </div>
      </div>
      <div class="va-skillrow">
        <div class="va-skill">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="M7 15l4-5 3 3 5-7"/></svg>
          <span>Tableau</span>
        </div>
        <div class="va-skill">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="color:#F2C811"><path d="M3 3v18h18"/><rect x="7" y="12" width="3" height="6" fill="currentColor"/><rect x="12" y="8" width="3" height="10" fill="currentColor"/><rect x="17" y="5" width="3" height="13" fill="currentColor"/></svg>
          <span>Power BI</span>
        </div>
        <div class="va-skill">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 21s-6-5.3-6-10a6 6 0 1112 0c0 4.7-6 10-6 10z"/><circle cx="12" cy="11" r="2.2"/></svg>
          <span>ArcGIS Pro</span>
        </div>
        <div class="va-skill">
          <svg viewBox="0 0 24 24" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="color:#00A1E0"><path d="M7 18a4.5 4.5 0 01-.6-8.96A6 6 0 0118 10a4 4 0 01-.5 8H7z"/></svg>
          <span>Salesforce</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS (auto-pulls everything in _portfolio) -->
<section class="va-section" id="projects">
  <div class="va-wrap">
    <h2>Featured projects</h2>
    <p class="va-sub">Selected analyses, each with the question, method, and findings.</p>
    <div class="va-projects">
      {% assign projects = site.portfolio | sort: 'date' | reverse %}
      {% for p in projects %}
        {% assign teaser = p.header.teaser | default: p.teaser %}
        <a class="va-project" href="{{ p.url | relative_url }}">
          <div class="va-thumb">
            {% if teaser %}
              {% assign first_char = teaser | slice: 0 %}
              {% if teaser contains '://' or first_char == '/' %}
                <img src="{{ teaser | relative_url }}" alt="{{ p.title }}">
              {% else %}
                <img src="{{ '/images/' | append: teaser | relative_url }}" alt="{{ p.title }}">
              {% endif %}
            {% endif %}
          </div>
          <div class="va-body">
            <h3>{{ p.title }}</h3>
            <p>{{ p.excerpt | strip_html | truncate: 230 }}</p>
          </div>
        </a>
      {% endfor %}
    </div>
    <p class="va-more"><a href="{{ '/portfolio/' | relative_url }}">See all projects &rarr;</a></p>
  </div>
</section>
