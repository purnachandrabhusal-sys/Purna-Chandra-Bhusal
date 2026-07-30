---
layout: default
title: Curriculum Vitae
lede: "The complete record — one click, no login."
permalink: /cv/
description: "Curriculum vitae of Purna [Surname] — PDF, viewable and downloadable."
---

<div class="cv-actions">
  <a class="btn btn-primary" href="{{ site.cv_file | relative_url }}" download>Download PDF</a>
  <a class="btn" href="{{ site.cv_file | relative_url }}" target="_blank" rel="noopener">Open in browser</a>
</div>

<p class="fine">Last updated {{ site.cv_updated }}. If a search committee needs anything further — transcripts, references, teaching evaluations — <a href="mailto:{{ site.email }}">email me</a>.</p>

<object class="cv-embed" data="{{ site.cv_file | relative_url }}" type="application/pdf" aria-label="Embedded CV PDF">
  <p>Your browser can’t preview PDFs here — use the <a href="{{ site.cv_file | relative_url }}">download button</a> above instead.</p>
</object>
