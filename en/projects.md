---
layout: default
title: Projects
lang: en
permalink: /en/projects/
translation: /projects/
---

# Projects

<p class="page-intro">Not every ticket deserves its own case study. These are the stories that best show how I work: make delivery predictable, remove repetitive work, and leave a clear process behind for the team.</p>

<section class="case-study">
  <p class="case-kicker">Core experience · TeamCity · CI/CD</p>
  <h2>Made delivery for 50+ services calm and repeatable</h2>
  <div class="case-grid">
    <div><h3>Starting point</h3><p>.NET and frontend services had different build and deployment steps. The failure was often not in the code, but in a manual action or an environment difference.</p></div>
    <div><h3>What changed</h3><p>I brought TeamCity CI/CD to a common approach: builds, tests, artefacts and deployment to Linux and Windows. Repetitive work moved into PowerShell, Bash and Python automation.</p></div>
    <div><h3>Outcome</h3><p>Release operations became 2–3 times faster, with 50–70% less manual involvement. When something failed, the team could see which stage needed attention. <a href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener">Public delivery patterns ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Platform operations · Docker · PostgreSQL</p>
  <h2>Built test environments that do not need to be assembled by hand</h2>
  <div class="case-grid">
    <div><h3>The need</h3><p>Branches, integrations and automated tests all need isolated environments. When the database, access and services are prepared manually, testing waits for infrastructure.</p></div>
    <div><h3>The approach</h3><p>I prepared TeamCity templates for Linux environments with Docker and PostgreSQL: restoring a test database, publishing the application, configuring access and running UI/API tests.</p></div>
    <div><h3>Outcome</h3><p>The path from a branch to a ready environment became repeatable. Build, access and infrastructure failures show up at a specific pipeline stage instead of after a long manual investigation. <a href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener">Public example and runbook ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Reliability · PostgreSQL · S3/MinIO · Observability</p>
  <h2>Restored services and made the next incident easier</h2>
  <div class="case-grid">
    <div><h3>Reality</h3><p>Across 30+ Linux and Windows servers, a problem rarely lives in one place. It can sit at the boundary of the application, network, reverse proxy, database and CI/CD.</p></div>
    <div><h3>How I worked</h3><p>I investigated the full path, aligned environment configuration, and put in health checks, logging and backups for PostgreSQL, configuration and files in S3/MinIO.</p></div>
    <div><h3>What remained</h3><p>Not just a restored service, but a clearer operating picture: metrics and logs in Zabbix, Grafana, ELK and Graylog, explicit checkpoints and a recovery path.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">DevSecOps · Security automation</p>
  <h2>Brought security checks into the normal development path</h2>
  <div class="case-grid">
    <div><h3>Why</h3><p>Vulnerability checks help only when their result is easy to understand before release, not when someone has to search through several unrelated reports.</p></div>
    <div><h3>What I did</h3><p>Connected Trivy, Semgrep, CodeQL and dependency analysis for different stacks. I also prepared a reproducible export of a public vulnerability catalogue with SHA-256 verification.</p></div>
    <div><h3>Outcome</h3><p>Checks became a clear CI stage instead of a noisy red build. <a href="https://github.com/lvipa/fstec-asutp-exporter" target="_blank" rel="noopener">Public automation example ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Self-hosted AI · FastAPI · MCP</p>
  <h2>Built local AI services that help with everyday work</h2>
  <div class="case-grid">
    <div><h3>Two practical cases</h3><p>The first turns a recording into text through an HTTP API. The second finds earlier decisions and task context in working chats.</p></div>
    <div><h3>What I built</h3><p>A FastAPI service using VOSK, ffmpeg, timestamps and observability; plus a webhook bot, full-text search and MCP-style context retrieval for Codex.</p></div>
    <div><h3>Why it matters</h3><p>Neither is an AI demo for its own sake: both save time on routine work and stay self-hosted. <a href="https://github.com/lvipa/vosk-smart-stt-api" target="_blank" rel="noopener">STT API ↗</a> · <a href="https://github.com/lvipa/express-chat-context" target="_blank" rel="noopener">context search ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Short project · HPC · Slurm · Ceph</p>
  <h2>Prepared a compute cluster for handover to operations</h2>
  <div class="case-grid">
    <div><h3>Context</h3><p>This was a separate university project, not my primary role. The clusters needed to be ready for safe day-to-day use.</p></div>
    <div><h3>What I did</h3><p>Checked Slurm and CephFS, set up a backup controller, CPU and memory limits, shared storage, and templates for VASP and Gaussian calculations.</p></div>
    <div><h3>Outcome</h3><p>A working queue, verified test calculations and a concise operational guide — without relying on the person who originally configured the cluster.</p></div>
  </div>
</section>

<h2 class="project-section-title">Public tools</h2>
<div class="project-links">
  <a class="project-link" href="https://github.com/lvipa/teamcity-scripts" target="_blank" rel="noopener"><strong>TeamCity REST API utilities ↗</strong><span>PowerShell tools for build-configuration and dependency analysis.</span></a>
  <a class="project-link" href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener"><strong>Platform Ops Lab ↗</strong><span>A sanitised example of branch environments, readiness gates and a runbook.</span></a>
  <a class="project-link" href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener"><strong>DevOps Delivery Lab ↗</strong><span>Release validation, health checks and an operations checklist.</span></a>
  <a class="project-link" href="https://github.com/lvipa/minichat-platform" target="_blank" rel="noopener"><strong>MiniChat Platform ↗</strong><span>A personal full-stack project: .NET, Angular PWA, Keycloak and SignalR.</span></a>
</div>

<p class="page-note">Corporate cases are intentionally anonymised: no company names, hosts, credentials or internal architecture.</p>
