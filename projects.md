---
layout: default
title: Проекты
permalink: /projects/
lang: ru
translation: /en/projects/
---

# Проекты

<p class="page-intro">Ключевые реализации из основной работы и отдельных проектов. Формат короткий: что именно построено и какой эффект это дало. Корпоративные названия, адреса и данные намеренно не публикую.</p>

<section class="case-study">
  <p class="case-kicker">Основной опыт · TeamCity · CI/CD</p>
  <h2>Поставка 50+ сервисов</h2>
  <div class="case-grid">
    <div><h3>Реализация</h3><ul><li>TeamCity build/deploy-конфигурации для .NET и frontend.</li><li>Сборка → тесты → публикация артефактов → деплой в Linux/Windows.</li><li>PowerShell, Bash и Python для повторяемых шагов.</li></ul></div>
    <div><h3>Конструкции платформы</h3><ul><li>Шаблоны и параметры сборок вместо отдельных ручных сценариев.</li><li>Branch filters, зависимости конфигураций и правила очистки артефактов.</li><li>Проверка влияния изменений через TeamCity REST API.</li></ul></div>
    <div><h3>Эффект</h3><p>Релизные операции стали быстрее в 2–3 раза, а ручное участие сократилось на 50–70%. <a href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener">Открытые паттерны поставки ↗</a></p></div>
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
    <div><h3>Эксплуатация</h3><ul><li>30+ Linux/Windows-серверов, контейнеры, Nginx/IIS.</li><li>PostgreSQL, Redis, S3/MinIO и файловые хранилища.</li><li>AD, DNS, GPO и сервисные учётные записи.</li></ul></div>
    <div><h3>Контроль и восстановление</h3><ul><li>Резервное копирование БД, конфигураций и файлов.</li><li>Health-check, единые каталоги и логирование.</li><li>Zabbix, Grafana, ELK и Graylog для метрик и журналов.</li></ul></div>
    <div><h3>Результат</h3><p>Сложные инциденты разбираются по цепочке «приложение → ОС → сеть → proxy → БД → CI/CD», а не наугад.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">DevSecOps · Security automation</p>
  <h2>Security checks в CI/CD</h2>
  <div class="case-grid">
    <div><h3>Инструменты</h3><ul><li>Trivy для SCA и контейнеров.</li><li>Semgrep и CodeQL для SAST.</li><li>Нормализация результатов и сводная отчётность.</li></ul></div>
    <div><h3>Реализация</h3><ul><li>Выборочная проверка нужного проекта и стека.</li><li>Раздельные отчёты для frontend, .NET, Python и legacy-кода.</li><li>Воспроизводимая выгрузка CVE-каталога с SHA-256.</li></ul></div>
    <div><h3>Результат</h3><p>Проверка безопасности стала отдельным понятным quality gate. <a href="https://github.com/lvipa/fstec-asutp-exporter" target="_blank" rel="noopener">Открытый пример ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Self-hosted AI · FastAPI · MCP</p>
  <h2>Self-hosted AI-сервисы</h2>
  <div class="case-grid">
    <div><h3>Speech-to-text</h3><ul><li>FastAPI + VOSK + ffmpeg.</li><li>Выбор модели, таймкоды, пунктуация, метрики.</li><li>Linux/Windows-развёртывание и нагрузочные замеры.</li></ul></div>
    <div><h3>Контекст для задач</h3><ul><li>Webhook-бот, SQLite FTS5 и API поиска.</li><li>Выдача фрагмента с датой и автором.</li><li>Подключение к Codex через skill/MCP-подход.</li></ul></div>
    <div><h3>Открытый код</h3><p><a href="https://github.com/lvipa/vosk-smart-stt-api" target="_blank" rel="noopener">STT API ↗</a><br><a href="https://github.com/lvipa/express-chat-context" target="_blank" rel="noopener">Поиск контекста ↗</a></p></div>
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
  <a class="project-link" href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener"><strong>Platform Ops Lab ↗</strong><span>Обезличенный пример тестовых сред, readiness-проверок и runbook.</span></a>
  <a class="project-link" href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener"><strong>DevOps Delivery Lab ↗</strong><span>Проверки релизов, health-check и эксплуатационный чек-лист.</span></a>
  <a class="project-link" href="https://github.com/lvipa/minichat-platform" target="_blank" rel="noopener"><strong>MiniChat Platform ↗</strong><span>Личный full-stack проект: .NET, Angular PWA, Keycloak и SignalR.</span></a>
</div>

<p class="page-note">Все рабочие кейсы намеренно обезличены: без названий компаний, адресов, учётных данных и внутренней архитектуры.</p>
