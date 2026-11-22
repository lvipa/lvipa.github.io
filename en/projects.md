---
layout: default
title: Projects
lang: en
permalink: /en/projects/
translation: /projects/
---

# Projects

<p class="page-intro">Work at SMS-IT and&nbsp;selected projects: builds, service deployment, authentication and&nbsp;data recovery. Implementation details and&nbsp;public tools are below. Internal addresses, configuration and&nbsp;data are not published.</p>

<section class="case-study">
  <p class="case-kicker">Core experience · TeamCity · CI/CD</p>
  <h2>Application builds and&nbsp;delivery with&nbsp;TeamCity</h2>
  <div class="case-grid">
    <div><h3>Build chains</h3><ul><li>Builds, tests, artefacts and&nbsp;deployment of&nbsp;.NET, Python and&nbsp;frontend applications to&nbsp;Linux/Windows.</li><li>EXE/DLL and&nbsp;installer signing tested in&nbsp;three chains: version → sign → verify → package.</li><li>Repeatable steps in&nbsp;PowerShell, Bash and&nbsp;Python.</li></ul></div>
    <div><h3>Automation</h3><ul><li>TeamCity templates, parameters and&nbsp;configuration dependencies.</li><li>Branch-filter synchronisation from deploy configurations to&nbsp;related build configurations through the REST API.</li><li>A Bash check after JDK updates: a systemd timer restarts the service only if its Java process uses a deleted executable.</li></ul></div>
    <div><h3>GitLab Runner</h3><p>Deployed the runner in&nbsp;Docker on Debian 12. Configured the Docker executor, private-registry access and&nbsp;a .NET SDK image for&nbsp;build jobs.</p><p><a href="https://github.com/lvipa/teamcity-branch-sync" target="_blank" rel="noopener">Generic branch-sync example ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Kubernetes · Keycloak · Portainer</p>
  <h2>Deploying services to&nbsp;Kubernetes</h2>
  <div class="case-grid">
    <div><h3>New Keycloak test environment</h3><ul><li>Official image, Secrets, resource limits and&nbsp;startup/readiness/liveness probes.</li><li>PostgreSQL database copy, schema-migration checks, rollout and&nbsp;OIDC endpoint checks.</li><li>MetalLB exposure, domain sign-in&nbsp;and&nbsp;scoped administration permissions.</li></ul></div>
    <div><h3>Portainer</h3><ul><li>Helm, persistent PV/PVC storage and&nbsp;HTTPS.</li><li>Six Docker hosts connected without restarting applications.</li><li>AD/LDAPS with&nbsp;certificate validation and&nbsp;restricted network access to&nbsp;agents.</li></ul></div>
    <div><h3>Scope</h3><p>Application deployment and&nbsp;maintenance in&nbsp;an existing Kubernetes cluster: configuration, persistent data, availability and&nbsp;authentication.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Platform operations · Docker · PostgreSQL</p>
  <h2>Branch environments and&nbsp;automated tests</h2>
  <div class="case-grid">
    <div><h3>Implementation</h3><ul><li>Linux environments: Docker Compose, PostgreSQL and&nbsp;application configuration.</li><li>Restore a known test database before each run.</li><li>UI/API execution, including Playwright.</li></ul></div>
    <div><h3>Access and&nbsp;lifecycle</h3><ul><li>Keycloak/OpenID integration for&nbsp;test environments.</li><li>Provisioning from a branch or&nbsp;TeamCity template.</li><li>Readiness gates, logs and&nbsp;artefacts for&nbsp;diagnosis.</li></ul></div>
    <div><h3>Outcome</h3><p>An environment can be rebuilt without a manual sequence of&nbsp;steps. <a href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener">Public example and&nbsp;runbook ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Reliability · PostgreSQL · S3/MinIO · Observability</p>
  <h2>Service and&nbsp;data reliability</h2>
  <div class="case-grid">
    <div><h3>Operations</h3><ul><li>Linux/Windows environments, containers and&nbsp;Nginx/IIS reverse proxies.</li><li>PostgreSQL, Redis, S3/MinIO and&nbsp;file storage.</li><li>AD, DNS, GPO and&nbsp;service identities.</li></ul></div>
    <div><h3>Updates and&nbsp;recovery</h3><ul><li>Tested TeamCity updates and&nbsp;rollback for&nbsp;three AI services, preserving models and&nbsp;data.</li><li>Test-database restoration from templates; database, configuration and&nbsp;file backups in&nbsp;S3/MinIO.</li><li>Zabbix checks model readiness, API availability and&nbsp;responses without uploading user documents.</li></ul></div>
    <div><h3>Diagnosis</h3><p>Investigated degradation across several environments, tracing the application, OS, network, reverse proxy, database and&nbsp;CI/CD. Removed the causes and&nbsp;standardised configuration.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">DevSecOps · Security automation</p>
  <h2>Security scans and&nbsp;consolidated reports</h2>
  <div class="case-grid">
    <div><h3>Tools</h3><ul><li>Trivy for&nbsp;SCA and&nbsp;containers.</li><li>Semgrep and&nbsp;CodeQL for&nbsp;SAST.</li><li>Normalised results and&nbsp;consolidated reporting.</li></ul></div>
    <div><h3>Implementation</h3><ul><li>PowerShell orchestration with&nbsp;project and&nbsp;scanner selection.</li><li>Reports for&nbsp;frontend, .NET and&nbsp;Python projects in&nbsp;JSON/SARIF and&nbsp;Excel.</li><li>A separate CVE-catalogue export tool with&nbsp;SHA-256.</li></ul></div>
    <div><h3>Public tools</h3><p>The scripts run selected scanners and&nbsp;collect their findings in&nbsp;a consolidated report for&nbsp;review.</p><p><a href="https://github.com/lvipa/security-scan-orchestrator" target="_blank" rel="noopener">Security Scan Orchestrator ↗</a> · <a href="https://github.com/lvipa/fstec-asutp-exporter" target="_blank" rel="noopener">FSTEC exporter ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Self-hosted AI · FastAPI · MCP</p>
  <h2>Self-hosted AI services</h2>
  <div class="case-grid">
    <div><h3>Speech-to-text</h3><ul><li>FastAPI + VOSK + ffmpeg.</li><li>Model choice, word timings, punctuation and&nbsp;metrics.</li><li>Linux/Windows deployment and&nbsp;load testing.</li></ul></div>
    <div><h3>Task context</h3><ul><li>Webhook bot, SQLite FTS5 and&nbsp;search API.</li><li>Returns a message fragment with&nbsp;date and&nbsp;author.</li><li>Connects to&nbsp;Codex through a skill/MCP approach.</li></ul></div>
    <div><h3>Public code</h3><p><a href="https://github.com/lvipa/vosk-smart-stt-api" target="_blank" rel="noopener">STT API ↗</a><br><a href="https://github.com/lvipa/meeting-transcription-service" target="_blank" rel="noopener">Meeting transcription service ↗</a><br><a href="https://github.com/lvipa/express-chat-context" target="_blank" rel="noopener">Context search ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Short project · HPC · Slurm · Ceph</p>
  <h2>HPC cluster: production handover</h2>
  <div class="case-grid">
    <div><h3>Scope</h3><p>Short university project: three 10-node clusters.</p></div>
    <div><h3>Implementation</h3><ul><li>Ceph/CephFS, Slurm, shared storage and&nbsp;scratch.</li><li>IPMI/iDRAC, BMC, Redfish API and&nbsp;inventory.</li><li>SONiC, Mellanox/NVIDIA Ethernet, VLAN and&nbsp;Jumbo Frames.</li></ul></div>
    <div><h3>Outcome</h3><p>Working queues, verified VASP/Gaussian calculations and&nbsp;operational documentation.</p></div>
  </div>
</section>

<h2 class="project-section-title">Public tools</h2>
<div class="project-links">
  <a class="project-link" href="https://github.com/lvipa/teamcity-scripts" target="_blank" rel="noopener"><strong>TeamCity REST API utilities ↗</strong><span>PowerShell tools for&nbsp;build-configuration and&nbsp;dependency analysis.</span></a>
  <a class="project-link" href="https://github.com/lvipa/teamcity-branch-sync" target="_blank" rel="noopener"><strong>TeamCity Branch Sync ↗</strong><span>Synchronises branch filters and&nbsp;build parameters through the REST API.</span></a>
  <a class="project-link" href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener"><strong>Platform Ops Lab ↗</strong><span>A sanitised example of&nbsp;branch environments, readiness gates and&nbsp;a runbook.</span></a>
  <a class="project-link" href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener"><strong>DevOps Delivery Lab ↗</strong><span>Release validation, health checks and&nbsp;an operations checklist.</span></a>
  <a class="project-link" href="https://github.com/lvipa/s3-retention-cleanup" target="_blank" rel="noopener"><strong>S3 Retention Cleanup ↗</strong><span>PowerShell utility for&nbsp;safe object cleanup with&nbsp;dry-run support and&nbsp;logging.</span></a>
  <a class="project-link" href="https://github.com/lvipa/minichat-platform" target="_blank" rel="noopener"><strong>MiniChat Platform ↗</strong><span>A personal full-stack project: .NET, Angular PWA, Keycloak and&nbsp;SignalR.</span></a>
</div>

<p class="page-note">Corporate cases are intentionally anonymised: no company names, hosts, credentials or&nbsp;internal architecture.</p>
