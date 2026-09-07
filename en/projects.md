---
layout: default
title: Projects
lang: en
permalink: /en/projects/
translation: /projects/
---

# Projects

<p class="page-intro">Key implementations from my main role and selected projects. Kept concise: what was built and what it changed. Company names, hosts and internal data are intentionally omitted.</p>

<section class="case-study">
  <p class="case-kicker">Core experience · TeamCity · CI/CD</p>
  <h2>Delivery for 50+ services</h2>
  <div class="case-grid">
    <div><h3>Implementation</h3><ul><li>TeamCity build/deploy configurations for .NET and frontend.</li><li>Build → test → artefact publishing → deployment to Linux/Windows.</li><li>Repeatable steps in PowerShell, Bash and Python.</li></ul></div>
    <div><h3>Platform patterns</h3><ul><li>Build templates and parameters instead of manual runbooks.</li><li>Branch filters, configuration dependencies and artefact-cleanup rules.</li><li>Change-impact analysis through the TeamCity REST API.</li></ul></div>
    <div><h3>Outcome</h3><p>Release operations became 2–3 times faster with 50–70% less manual involvement. <a href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener">Public delivery patterns ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Platform operations · Docker · PostgreSQL</p>
  <h2>Branch environments and automated tests</h2>
  <div class="case-grid">
    <div><h3>Implementation</h3><ul><li>Linux environments: Docker Compose, PostgreSQL and application configuration.</li><li>Restore a known test database before each run.</li><li>UI/API execution, including Playwright.</li></ul></div>
    <div><h3>Access and lifecycle</h3><ul><li>Keycloak/OpenID integration for test environments.</li><li>Provisioning from a branch or TeamCity template.</li><li>Readiness gates, logs and artefacts for diagnosis.</li></ul></div>
    <div><h3>Outcome</h3><p>An environment can be rebuilt without a manual sequence of steps. <a href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener">Public example and runbook ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Reliability · PostgreSQL · S3/MinIO · Observability</p>
  <h2>Service and data reliability</h2>
  <div class="case-grid">
    <div><h3>Operations</h3><ul><li>30+ Linux/Windows servers, containers, Nginx/IIS.</li><li>PostgreSQL, Redis, S3/MinIO and file storage.</li><li>AD, DNS, GPO and service identities.</li></ul></div>
    <div><h3>Control and recovery</h3><ul><li>Backups for databases, configuration and files.</li><li>Health checks, consistent directories and logging.</li><li>Zabbix, Grafana, ELK and Graylog for metrics and logs.</li></ul></div>
    <div><h3>Outcome</h3><p>Complex incidents are investigated across the application → OS → network → proxy → database → CI/CD path, rather than by guesswork.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">DevSecOps · Security automation</p>
  <h2>Security checks in CI/CD</h2>
  <div class="case-grid">
    <div><h3>Tools</h3><ul><li>Trivy for SCA and containers.</li><li>Semgrep and CodeQL for SAST.</li><li>Normalised results and consolidated reporting.</li></ul></div>
    <div><h3>Implementation</h3><ul><li>Targeted scans by project and stack.</li><li>Separate reports for frontend, .NET, Python and legacy code.</li><li>Reproducible CVE-catalogue export with SHA-256.</li></ul></div>
    <div><h3>Outcome</h3><p>Security became a clear quality gate in CI. <a href="https://github.com/lvipa/security-scan-orchestrator" target="_blank" rel="noopener">Security Scan Orchestrator ↗</a> · <a href="https://github.com/lvipa/fstec-asutp-exporter" target="_blank" rel="noopener">FSTEC exporter ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Self-hosted AI · FastAPI · MCP</p>
  <h2>Self-hosted AI services</h2>
  <div class="case-grid">
    <div><h3>Speech-to-text</h3><ul><li>FastAPI + VOSK + ffmpeg.</li><li>Model choice, word timings, punctuation and metrics.</li><li>Linux/Windows deployment and load testing.</li></ul></div>
    <div><h3>Task context</h3><ul><li>Webhook bot, SQLite FTS5 and search API.</li><li>Returns a message fragment with date and author.</li><li>Connects to Codex through a skill/MCP approach.</li></ul></div>
    <div><h3>Public code</h3><p><a href="https://github.com/lvipa/vosk-smart-stt-api" target="_blank" rel="noopener">STT API ↗</a><br><a href="https://github.com/lvipa/meeting-transcription-service" target="_blank" rel="noopener">Meeting transcription service ↗</a><br><a href="https://github.com/lvipa/express-chat-context" target="_blank" rel="noopener">Context search ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Short project · HPC · Slurm · Ceph</p>
  <h2>HPC cluster: production handover</h2>
  <div class="case-grid">
    <div><h3>Scope</h3><p>Short university project: three 10-node clusters.</p></div>
    <div><h3>Implementation</h3><ul><li>Ceph/CephFS, Slurm, shared storage and scratch.</li><li>IPMI/iDRAC, BMC, Redfish API and inventory.</li><li>SONiC, Mellanox/NVIDIA Ethernet, VLAN and Jumbo Frames.</li></ul></div>
    <div><h3>Outcome</h3><p>Working queues, verified VASP/Gaussian calculations and operational documentation.</p></div>
  </div>
</section>

<h2 class="project-section-title">Public tools</h2>
<div class="project-links">
  <a class="project-link" href="https://github.com/lvipa/teamcity-scripts" target="_blank" rel="noopener"><strong>TeamCity REST API utilities ↗</strong><span>PowerShell tools for build-configuration and dependency analysis.</span></a>
  <a class="project-link" href="https://github.com/lvipa/teamcity-branch-sync" target="_blank" rel="noopener"><strong>TeamCity Branch Sync ↗</strong><span>Synchronises branch filters and build parameters through the REST API.</span></a>
  <a class="project-link" href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener"><strong>Platform Ops Lab ↗</strong><span>A sanitised example of branch environments, readiness gates and a runbook.</span></a>
  <a class="project-link" href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener"><strong>DevOps Delivery Lab ↗</strong><span>Release validation, health checks and an operations checklist.</span></a>
  <a class="project-link" href="https://github.com/lvipa/s3-retention-cleanup" target="_blank" rel="noopener"><strong>S3 Retention Cleanup ↗</strong><span>PowerShell utility for safe object cleanup with dry-run support and logging.</span></a>
  <a class="project-link" href="https://github.com/lvipa/minichat-platform" target="_blank" rel="noopener"><strong>MiniChat Platform ↗</strong><span>A personal full-stack project: .NET, Angular PWA, Keycloak and SignalR.</span></a>
</div>

<p class="page-note">Corporate cases are intentionally anonymised: no company names, hosts, credentials or internal architecture.</p>
