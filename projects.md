---
layout: default
title: Проекты
permalink: /projects/
lang: ru
translation: /en/projects/
---

# Проекты

<p class="page-intro">Задачи из работы в СМС-ИТ и отдельных проектов: сборки, развёртывание сервисов, авторизация и восстановление данных. Ниже — детали реализации и ссылки на открытые инструменты. Рабочие адреса, конфигурации и данные не публикую.</p>

<section class="case-study">
  <p class="case-kicker">Основной опыт · TeamCity · CI/CD</p>
  <h2>Сборка и поставка приложений через TeamCity</h2>
  <div class="case-grid">
    <div><h3>Сборочные цепочки</h3><ul><li>Сборка, тестирование, артефакты и деплой .NET-, Python- и frontend-приложений в Linux/Windows.</li><li>Подписание EXE/DLL и установщиков проверено в трёх цепочках: версия → подпись → проверка → упаковка.</li><li>PowerShell, Bash и Python для повторяемых шагов.</li></ul></div>
    <div><h3>Автоматизация</h3><ul><li>Шаблоны, параметры и зависимости конфигураций TeamCity.</li><li>Синхронизация branch filters от deploy-конфигураций к связанным build-конфигурациям через REST API.</li><li>Bash-проверка процесса Java после обновления JDK: systemd timer перезапускает службу только при обнаружении удалённого исполняемого файла.</li></ul></div>
    <div><h3>GitLab Runner</h3><p>Развернул runner в Docker на Debian 12. Настроил Docker executor, доступ к приватному registry и использование образа .NET SDK для сборочных задач.</p><p><a href="https://github.com/lvipa/teamcity-branch-sync" target="_blank" rel="noopener">Обобщённый пример синхронизации веток ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Kubernetes · Keycloak · Portainer</p>
  <h2>Развёртывание сервисов в Kubernetes</h2>
  <div class="case-grid">
    <div><h3>Новый стенд Keycloak</h3><ul><li>Официальный образ, Secrets, ограничения ресурсов и startup/readiness/liveness probes.</li><li>Копия PostgreSQL-базы и проверка миграции схемы, rollout и OIDC endpoints.</li><li>Публикация через MetalLB; доменный вход и разграничение административных прав.</li></ul></div>
    <div><h3>Portainer</h3><ul><li>Helm, постоянное хранилище PV/PVC и HTTPS.</li><li>Подключение шести Docker-хостов без перезапуска приложений.</li><li>AD/LDAPS с проверкой сертификата; ограничение сетевого доступа к агентам.</li></ul></div>
    <div><h3>Область работы</h3><p>Развёртывание и сопровождение прикладных сервисов в существующем Kubernetes-кластере: конфигурация, хранение данных, доступность и авторизация.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Platform operations · Docker · PostgreSQL</p>
  <h2>Тестовые среды для веток и автотестов</h2>
  <div class="case-grid">
    <div><h3>Реализация</h3><ul><li>Linux-стенды: Docker Compose, PostgreSQL, конфигурация приложения.</li><li>Восстановление тестовой БД перед прогоном.</li><li>UI/API-прогоны, включая Playwright.</li></ul></div>
    <div><h3>Доступ и жизненный цикл</h3><ul><li>Интеграция тестовых контуров с Keycloak/OpenID.</li><li>Подготовка стенда из ветки или шаблона TeamCity.</li><li>Проверки готовности, логи и артефакты для диагностики.</li></ul></div>
    <div><h3>Эффект</h3><p>Стенд можно собрать повторно без ручной последовательности действий. <a href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener">Публичный пример и runbook ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Reliability · PostgreSQL · S3/MinIO · Observability</p>
  <h2>Надёжность сервисов и данных</h2>
  <div class="case-grid">
    <div><h3>Эксплуатация</h3><ul><li>Linux/Windows-среды, контейнеры и reverse proxy на Nginx/IIS.</li><li>PostgreSQL, Redis, S3/MinIO и файловые хранилища.</li><li>AD, DNS, GPO и сервисные учётные записи.</li></ul></div>
    <div><h3>Обновление и восстановление</h3><ul><li>Для трёх AI-сервисов проверены обновление и откат через TeamCity с сохранением данных и моделей.</li><li>Восстановление тестовых БД из шаблонов; резервные копии БД, конфигураций и файлов в S3/MinIO.</li><li>Zabbix проверяет готовность модели, API и ответ сервиса без загрузки пользовательских документов.</li></ul></div>
    <div><h3>Диагностика</h3><p>При деградации системы на нескольких контурах проверил приложение, ОС, сеть, reverse proxy, базу данных и CI/CD. Устранил причины и привёл конфигурации к единому виду.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">DevSecOps · Security automation</p>
  <h2>Запуск проверок безопасности и сводные отчёты</h2>
  <div class="case-grid">
    <div><h3>Инструменты</h3><ul><li>Trivy для SCA и контейнеров.</li><li>Semgrep и CodeQL для SAST.</li><li>Нормализация результатов и сводная отчётность.</li></ul></div>
    <div><h3>Реализация</h3><ul><li>PowerShell-оркестрация: выбор проекта и набора сканеров.</li><li>Отчёты для frontend-, .NET- и Python-проектов в JSON/SARIF и Excel.</li><li>Отдельный инструмент выгрузки CVE-каталога с SHA-256.</li></ul></div>
    <div><h3>Открытые инструменты</h3><p>Скрипты запускают выбранные сканеры и собирают результаты в сводный отчёт для разбора найденных проблем.</p><p><a href="https://github.com/lvipa/security-scan-orchestrator" target="_blank" rel="noopener">Security Scan Orchestrator ↗</a> · <a href="https://github.com/lvipa/fstec-asutp-exporter" target="_blank" rel="noopener">FSTEC exporter ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Self-hosted AI · FastAPI · MCP</p>
  <h2>Self-hosted AI-сервисы</h2>
  <div class="case-grid">
    <div><h3>Speech-to-text</h3><ul><li>FastAPI + VOSK + ffmpeg.</li><li>Выбор модели, таймкоды, пунктуация, метрики.</li><li>Linux/Windows-развёртывание и нагрузочные замеры.</li></ul></div>
    <div><h3>Контекст для задач</h3><ul><li>Webhook-бот, SQLite FTS5 и API поиска.</li><li>Выдача фрагмента с датой и автором.</li><li>Подключение к Codex через skill/MCP-подход.</li></ul></div>
    <div><h3>Открытый код</h3><p><a href="https://github.com/lvipa/vosk-smart-stt-api" target="_blank" rel="noopener">STT API ↗</a><br><a href="https://github.com/lvipa/meeting-transcription-service" target="_blank" rel="noopener">Сервис транскрибации ↗</a><br><a href="https://github.com/lvipa/express-chat-context" target="_blank" rel="noopener">Поиск контекста ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Краткосрочный проект · HPC · Slurm · Ceph</p>
  <h2>HPC-кластер: ввод в эксплуатацию</h2>
  <div class="case-grid">
    <div><h3>Масштаб</h3><p>Краткосрочный проект для университета: три 10-узловых кластера.</p></div>
    <div><h3>Реализация</h3><ul><li>Ceph/CephFS, Slurm, shared storage и scratch.</li><li>IPMI/iDRAC, BMC, Redfish API, инвентаризация.</li><li>SONiC, Mellanox/NVIDIA Ethernet, VLAN и Jumbo Frames.</li></ul></div>
    <div><h3>Результат</h3><p>Рабочие очереди, проверенные расчёты VASP/Gaussian и эксплуатационная документация.</p></div>
  </div>
</section>

<h2 class="project-section-title">Публичные инструменты</h2>
<div class="project-links">
  <a class="project-link" href="https://github.com/lvipa/teamcity-scripts" target="_blank" rel="noopener"><strong>TeamCity REST API utilities ↗</strong><span>PowerShell-инструменты для анализа конфигураций и зависимостей сборок.</span></a>
  <a class="project-link" href="https://github.com/lvipa/teamcity-branch-sync" target="_blank" rel="noopener"><strong>TeamCity Branch Sync ↗</strong><span>Синхронизация branch filters и параметров сборок через REST API.</span></a>
  <a class="project-link" href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener"><strong>Platform Ops Lab ↗</strong><span>Обезличенный пример тестовых сред, readiness-проверок и runbook.</span></a>
  <a class="project-link" href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener"><strong>DevOps Delivery Lab ↗</strong><span>Проверки релизов, health-check и эксплуатационный чек-лист.</span></a>
  <a class="project-link" href="https://github.com/lvipa/s3-retention-cleanup" target="_blank" rel="noopener"><strong>S3 Retention Cleanup ↗</strong><span>PowerShell-утилита для безопасной очистки объектов с dry-run и логированием.</span></a>
  <a class="project-link" href="https://github.com/lvipa/minichat-platform" target="_blank" rel="noopener"><strong>MiniChat Platform ↗</strong><span>Личный full-stack проект: .NET, Angular PWA, Keycloak и SignalR.</span></a>
</div>

<p class="page-note">Все рабочие кейсы намеренно обезличены: без названий компаний, адресов, учётных данных и внутренней архитектуры.</p>
