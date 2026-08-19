---
layout: default
title: Notes
lang: en
permalink: /en/notes/
translation: /notes/
---

# Notes

<p class="page-intro">Short working notes on practices that make infrastructure more predictable and delivery safer.</p>

<article class="note-card"><p class="case-kicker">Security scanning</p><h2>A security gate should not break delivery</h2><p>A scanner becomes useful when it can run on a focused scope and reports from different repositories and builds remain isolated. Generated-artifact exclusions, explicit paths and developer-friendly findings matter.</p></article>

<article class="note-card"><p class="case-kicker">Configuration management</p><h2>Idempotent deployment beats a long list of defaults</h2><p>When deployment creates missing sections and attributes itself, configuration remains compact. It reduces manual work and makes repeated execution safe.</p></article>

<article class="note-card"><p class="case-kicker">Databases · CI</p><h2>Test database restore is part of the pipeline contract</h2><p>A reproducible run starts with a known data state. Validate the backup, check the restore exit code and distinguish non-fatal warnings from actual failures.</p></article>

<article class="note-card"><p class="case-kicker">Release engineering</p><h2>Artifact composition is a signal, just like build status</h2><p>Comparing a new release with a reference can reveal accidental dependencies, debug files and packaging changes. A separate quality gate is often better than turning the main build red.</p></article>

<article class="note-card"><p class="case-kicker">HA · Observability</p><h2>Measure configuration drift instead of debating it</h2><p>Reference settings and regular comparison with runtime parameters turn an audit into a concrete list of deviations. Network and other environment-specific values should be separated from meaningful drift.</p></article>
