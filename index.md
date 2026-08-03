---
layout: default
hide_title: true
permalink: /
---

<!-- ================================================================
     HOME PAGE
     Lines you can safely edit are marked with  EDIT:
     Everything in [square brackets] is a placeholder to replace.
     ================================================================ -->

<section class="hero">
  <p class="eyebrow">Rhetoric &amp; Writing Studies</p> <!-- EDIT: field label -->

  <h1>{{ site.author_name }}</h1>

  <!-- EDIT: your two-sentence introduction. Keep it short — this is the
       first thing a search committee reads. -->
  <p class="intro">Scholar of [rhetoric, writing studies, and — one phrase naming your research focus]. I completed my PhD in Rhetoric and Writing Studies at The University of Texas at El Paso in [2026], where my dissertation examined [one plain-language sentence about the dissertation].</p>

  <div class="hero-actions">
    <a class="btn btn-primary" href="{{ site.cv_file | relative_url }}">Download CV (PDF)</a>
    <a class="btn" href="mailto:{{ site.email }}">Email me</a>
    {% if site.scholar_url != "" %}<a class="btn" href="{{ site.scholar_url }}">Google Scholar</a>{% endif %}
    {% if site.orcid_url != "" %}<a class="btn" href="{{ site.orcid_url }}">ORCID</a>{% endif %}
  </div>
</section>

<section class="verify" aria-label="Credentials at a glance">
  <p class="verify-label">At a glance — for search committees</p>
  <dl class="verify-grid">
    <div>
      <dt>Degree</dt>
      <dd>PhD, Rhetoric &amp; Writing Studies, The University of Texas at El Paso, [2026]</dd> <!-- EDIT -->
    </div>
    <div>
      <dt>Dissertation</dt>
      <dd>“[Dissertation title]” — directed by [Advisor name]</dd> <!-- EDIT -->
    </div>
    <div>
      <dt>Research areas</dt>
      <dd>[Area 1] · [Area 2] · [Area 3]</dd> <!-- EDIT -->
    </div>
    <div>
      <dt>Teaching</dt>
      <dd>[N] semesters of first-year composition and [other courses] at UTEP</dd> <!-- EDIT -->
    </div>
    <div>
      <dt>Publications</dt>
      <dd>[N] peer-reviewed articles — <a href="{{ '/publications/' | relative_url }}">see the list</a></dd> <!-- EDIT -->
    </div>
    <div>
      <dt>Contact</dt>
      <dd><a href="mailto:{{ site.email }}">{{ site.email }}</a> · references available on request</dd>
    </div>
  </dl>
</section>

## Selected publications

<!-- EDIT: keep the 2–3 strongest items here. The full list lives on the
     Publications page. Write each as a normal citation on its own "-" line. -->

- [Surname], P. ([Year]). [Article title]. *[Journal Name]*, [volume]([issue]), [pages]. [https://doi.org/xxxx](https://doi.org/xxxx)
- [Surname], P. ([Year]). [Chapter title]. In [Editor] (Ed.), *[Book title]* (pp. [pages]). [Publisher].

[All publications →]({{ '/publications/' | relative_url }})

## Teaching

<!-- EDIT: one short paragraph. Details belong on the Teaching page. -->

I have taught [first-year composition, technical writing, and …] at [The University of Texas at El Paso], with a teaching approach grounded in [one phrase — e.g., accessible, translingual, community-engaged pedagogy].

[Teaching portfolio →]({{ '/teaching/' | relative_url }})

## Currently

<!-- EDIT: one line of news. Update it every month or two so the site
     looks alive — e.g. "On the 2026–27 academic job market" or
     "Presenting at CCCC 2027, Chicago." Delete this section if unused. -->

On the [2026–27] academic job market for tenure-track and postdoctoral positions in rhetoric, composition, and writing studies.
