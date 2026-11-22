---
layout: default
title: Resume - Ivan Lipatov
description: Senior DevOps & Infrastructure Engineer - experience, skills and downloadable resumes.
permalink: /en/resume/
lang: en
translation: /resume/
---

<section class="resume-page shell">
  <div class="resume-head">
    <div>
      <p class="resume-kicker">Senior DevOps &amp; Infrastructure Engineer</p>
      <h1>Ivan Lipatov</h1>
      <p>Samara, Russia · Open to remote and hybrid roles</p>
      <p class="resume-links"><a href="mailto:lvipa@ivanlipatov.ru">Email</a><a href="https://t.me/lvipa">Telegram</a><a href="https://github.com/lvipa">GitHub</a><a href="https://www.linkedin.com/in/lvipa/">LinkedIn</a></p>
    </div>
    <img src="{{ '/assets/images/ivan-lipatov.jpeg' | relative_url }}" alt="Ivan Lipatov" class="resume-photo">
  </div>

  <section class="resume-highlights" aria-label="Core areas">
    <div><strong>Since 2017</strong><span>working in IT</span></div>
    <div><strong>Since 2020</strong><span>at SMS-IT</span></div>
    <div><strong>CI/CD</strong><span>TeamCity and build automation</span></div>
    <div><strong>Docker</strong><span>Compose and Kubernetes</span></div>
    <div><strong>Scripting</strong><span>PowerShell, Bash, Python</span></div>
  </section>

  <div class="resume-layout">
    <div class="resume-main">
      <h2>Work experience</h2>
      <section class="resume-employer-group" aria-label="Core experience at SMS-IT">
        <header class="resume-employer-head">
          <p>September 2020 — present</p>
          <h3>SMS-Information Technologies LLC</h3>
          <span>From customer implementations to CI/CD and internal infrastructure</span>
        </header>

        <article class="resume-job resume-job--current">
          <h3>Lead IS Implementation Specialist / Senior DevOps &amp; Infrastructure Engineer</h3>
          <p class="resume-meta">Feb 2024 - present · Samara, Russia</p>
          <p>Develop CI/CD and maintain the company's internal infrastructure: application builds and delivery, test environments, and Linux and Windows servers.</p>
          <ul>
            <li>Configure and maintain TeamCity builds, tests and deployments for .NET, Python and frontend applications. Automated branch synchronisation between deploy and build configurations through the REST API.</li>
            <li>Implemented and tested EXE/DLL and installer signing in three build chains, including version changes, signature verification and packaging.</li>
            <li>Deployed GitLab Runner in Docker on Debian 12 with the Docker executor, a private registry and a .NET SDK image.</li>
            <li>Deployed a new Keycloak test environment in Kubernetes. Tested migration of a PostgreSQL database copy and configured Secrets, probes, container resources and MetalLB exposure.</li>
            <li>Deployed Portainer through Helm with PV/PVC storage and HTTPS. Connected six Docker hosts without restarting applications; configured AD/LDAPS and network restrictions for agents.</li>
            <li>Configured test-environment authentication through Keycloak/OIDC and ADFS, including claims, groups, roles and user sign-in checks.</li>
            <li>Configured TeamCity updates and rollback for three AI services, preserving models and data. Added Zabbix readiness checks that do not send user documents.</li>
            <li>Automated test-database restoration from templates. Maintain PostgreSQL, Redis, S3/MinIO, Nginx/IIS, backups and monitoring.</li>
            <li>Developed PowerShell tools to run Trivy, Semgrep and CodeQL and consolidate JSON/SARIF and Excel reports. Deployed VOSK/FastAPI and a transcription service.</li>
          </ul>
          <p><a href="{{ '/en/projects/' | relative_url }}">Implementation details and public examples →</a></p>
          <div class="resume-project-note">
            <h4>Additional project work · March — June 2026</h4>
            <p>Alongside my main job, commissioned three 10-node HPC clusters for Samara State Technical University: Linux, Slurm, Ceph/CephFS and SONiC networking. Configured storage and job queues, investigated hardware and network failures, and wrote operational documentation.</p>
          </div>
        </article>

        <article class="resume-job">
          <h3>Senior Implementation Service Specialist</h3>
          <p class="resume-meta">Dec 2021 - Jan 2024 · Samara, Russia</p>
          <ul>
            <li>Resolved a complex degradation incident affecting several corporate system environments: traced the chain from application to database and CI/CD, removed root causes and standardized configuration.</li>
            <li>Implemented and operated an enterprise system for large customers: Windows/Debian, IIS, .NET Core, PostgreSQL, Redis Cluster, Docker, Ceph, MinIO and S3.</li>
            <li>Agreed technical solutions with customer security and engineering teams; contributed to deployment automation, monitoring and backups.</li>
          </ul>
        </article>

        <article class="resume-job">
          <h3>Implementation Service Specialist</h3>
          <p class="resume-meta">Sep 2020 - Nov 2021 · Samara, Russia</p>
          <ul>
            <li>Prepared test and server environments for SCADA and analytics systems; performed load and stress testing, analysed metrics and helped address bottlenecks.</li>
            <li>Administered Windows Server and PostgreSQL; contributed to Docker, Ceph, MinIO, S3 storage, monitoring and backup configuration.</li>
          </ul>
        </article>
      </section>

      <article class="resume-job">
        <h3>Implementation &amp; Technical Support Specialist</h3>
        <p class="resume-company">InfoPro Group of Companies</p>
        <p class="resume-meta">Sep 2017 - Aug 2019 · Samara, Russia</p>
        <ul><li>Implemented energy-sector software, configuring calculation workflows, algorithms and reports.</li><li>Automated data collection and processing in C#, including HTTP requests and file processing. Worked with SQL, PostgreSQL and MS SQL Server.</li><li>Investigated bugs, tested functionality, wrote instructions and supported users.</li></ul>
      </article>
    </div>
    <aside class="resume-side">
      <h2>Education</h2><p><strong>Samara State Technical University</strong><br>Higher education, Mathematical Support and Administration of Information Systems<br>2017</p>
      <h2>Skills</h2>
      <p><strong>CI/CD:</strong> TeamCity, GitLab Runner, REST API, Git</p>
      <p><strong>Containers:</strong> Docker, Docker Compose, Kubernetes, Helm, Portainer</p>
      <p><strong>Systems &amp; scripting:</strong> Linux, Windows Server, Bash, PowerShell, Python, systemd</p>
      <p><strong>Data:</strong> PostgreSQL, Redis, S3/MinIO, Ceph/CephFS</p>
      <p><strong>Monitoring:</strong> Zabbix, Grafana, ELK, Graylog</p>
      <p><strong>Networking &amp; access:</strong> Nginx, IIS, DNS, TLS, AD, GPO, Keycloak, OIDC, ADFS</p>
      <p><strong>Security scanning:</strong> Trivy, Semgrep, CodeQL</p>
      <p><strong>Basic experience:</strong> Ansible — test tasks</p>
      <h2>Languages</h2><p>Russian — Native<br>English — B1 (Intermediate)</p>
      <h2>Download PDF</h2><p class="resume-downloads"><a class="button button-primary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_EN.pdf' | relative_url }}">English version</a><a class="button button-secondary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_RU.pdf' | relative_url }}">Russian version</a></p>
    </aside>
  </div>
</section>
