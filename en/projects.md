---
layout: default
title: Projects
lang: en
permalink: /en/projects/
translation: /projects/
---

# Projects

<p class="page-intro">An anonymized selection of infrastructure and DevOps work: cluster reliability, CI/CD, test environments and engineering quality gates.</p>

<section class="case-study"><p class="case-kicker">CI/CD · Security</p><h2>Security scanning in the build pipeline</h2><div class="case-grid"><div><h3>Challenge</h3><p>Surface dependency and code risks early, without waiting for an external audit.</p></div><div><h3>Approach</h3><p>Built SCA/SAST workflows with Trivy, Semgrep, CodeQL and dependency checks; added solution-targeted runs, separate report directories and generated-file exclusions.</p></div><div><h3>Outcome</h3><p>A repeatable security workflow for frontend, backend and legacy code, with no cross-run report pollution.</p></div></div></section>

<section class="case-study"><p class="case-kicker">PostgreSQL · HA · Compliance</p><h2>HA cluster configuration drift control</h2><div class="case-grid"><div><h3>Challenge</h3><p>Reduce the risk of divergence between a PostgreSQL HA reference configuration and the live cluster.</p></div><div><h3>Approach</h3><p>Automated comparison of etcd, Patroni, HAProxy and Keepalived configurations, including PostgreSQL runtime settings while filtering comments and environment-specific values.</p></div><div><h3>Outcome</h3><p>A practical technical audit that highlights deviations before they become incidents.</p></div></div></section>

<section class="case-study"><p class="case-kicker">Linux · TeamCity · Testing</p><h2>Linux migration for test environments</h2><div class="case-grid"><div><h3>Challenge</h3><p>Move environments and automated tests to a consistent Linux platform without losing reproducibility.</p></div><div><h3>Approach</h3><p>Prepared systemd services, Docker deployment, PostgreSQL configuration and a deterministic sequence: database restore → deploy → UI tests → API tests.</p></div><div><h3>Outcome</h3><p>A production-oriented test environment that is easier to repeat and diagnose.</p></div></div></section>

<section class="case-study"><p class="case-kicker">Release engineering · Quality gate</p><h2>Build artifact composition control</h2><div class="case-grid"><div><h3>Challenge</h3><p>Detect unexpected files in release artifacts before delivery.</p></div><div><h3>Approach</h3><p>Created a separate CI check that compares current and reference artifacts, including nested ZIP archives.</p></div><div><h3>Outcome</h3><p>The team receives a file diff and notification while the main build remains independent from review.</p></div></div></section>

<section class="case-study"><p class="case-kicker">SonarQube · Build agents</p><h2>Portable code-quality analysis</h2><div class="case-grid"><div><h3>Challenge</h3><p>Run C# analysis reliably across build agents with different environments.</p></div><div><h3>Approach</h3><p>Standardized the JDK and scanner tooling, environment variables, certificate trust and reverse-proxy limits for larger reports.</p></div><div><h3>Outcome</h3><p>Quality analysis becomes a normal CI capability rather than a feature of one special agent.</p></div></div></section>

<p class="page-note">All examples are intentionally anonymized: no company names, hosts, credentials or internal topology.</p>
