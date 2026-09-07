---
layout: default
title: Проекты
permalink: /projects/
lang: ru
translation: /en/projects/
---

# Проекты

<p class="page-intro">Не все рабочие задачи стоит превращать в отдельную карточку. Здесь — несколько историй, которые лучше всего показывают мой подход: сначала сделать работу команды предсказуемой, затем убрать ручной труд и оставить после себя понятный процесс.</p>

<section class="case-study">
  <p class="case-kicker">Основной опыт · TeamCity · CI/CD</p>
  <h2>Сделал поставку 50+ сервисов спокойной и повторяемой</h2>
  <div class="case-grid">
    <div><h3>С чего начал</h3><p>У разных .NET- и frontend-сервисов были свои шаги сборки и деплоя. Ошибку легко было получить не в коде, а в ручном действии или отличии окружения.</p></div>
    <div><h3>Что изменил</h3><p>Привёл CI/CD в TeamCity к общему подходу: сборка, тесты, артефакты и деплой в Linux и Windows. Рутинные шаги автоматизировал на PowerShell, Bash и Python.</p></div>
    <div><h3>Что это дало</h3><p>Релизные операции стали быстрее в 2–3 раза, а ручное участие сократилось на 50–70%. При проблеме стало понятно, на каком шаге искать причину. <a href="https://github.com/lvipa/devops-delivery-lab" target="_blank" rel="noopener">Открытые паттерны поставки ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Platform operations · Docker · PostgreSQL</p>
  <h2>Настроил тестовые среды, которые не нужно собирать вручную</h2>
  <div class="case-grid">
    <div><h3>Задача</h3><p>Для веток, новых интеграций и автотестов нужны отдельные среды. Когда базу, доступ и сервисы поднимают вручную, проверки начинают ждать инфраструктуру.</p></div>
    <div><h3>Решение</h3><p>Подготовил шаблоны TeamCity для Linux-сред с Docker и PostgreSQL: восстановление тестовой базы, публикация приложения, настройка доступа и запуск UI/API-тестов.</p></div>
    <div><h3>Результат</h3><p>Путь от ветки до готового стенда стал повторяемым. Ошибки сборки, доступа и инфраструктуры видны в конкретном шаге пайплайна, а не после долгой ручной диагностики. <a href="https://github.com/lvipa/platform-ops-lab" target="_blank" rel="noopener">Публичный пример и runbook ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Reliability · PostgreSQL · S3/MinIO · Observability</p>
  <h2>Возвращал сервисы в рабочее состояние и делал следующие инциденты проще</h2>
  <div class="case-grid">
    <div><h3>Реальность</h3><p>В инфраструктуре из 30+ Linux/Windows-серверов проблема редко живёт в одном месте: она может быть на стыке приложения, сети, reverse proxy, базы и CI/CD.</p></div>
    <div><h3>Как работал</h3><p>Разбирал цепочку целиком, выравнивал конфигурации окружений, настраивал health-check, логирование и резервное копирование PostgreSQL, конфигураций и файлов в S3/MinIO.</p></div>
    <div><h3>Что оставалось после</h3><p>Не только восстановленный сервис, но и более ясная картина: метрики и логи в Zabbix, Grafana, ELK и Graylog, понятные точки проверки и сценарий восстановления.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">DevSecOps · Security automation</p>
  <h2>Встроил проверки безопасности в обычный путь разработки</h2>
  <div class="case-grid">
    <div><h3>Зачем</h3><p>Проверка уязвимостей полезна только тогда, когда её результат можно быстро понять до релиза, а не искать вручную в нескольких разрозненных отчётах.</p></div>
    <div><h3>Что сделал</h3><p>Подключил Trivy, Semgrep, CodeQL и анализ зависимостей для разных стеков. Дополнительно подготовил воспроизводимую выгрузку публичного каталога уязвимостей с контролем SHA-256.</p></div>
    <div><h3>Итог</h3><p>Проверки стали отдельным понятным этапом CI, а не «шумной» красной сборкой. <a href="https://github.com/lvipa/fstec-asutp-exporter" target="_blank" rel="noopener">Открытый пример автоматизации ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Self-hosted AI · FastAPI · MCP</p>
  <h2>Запускал локальные AI-сервисы, полезные в ежедневной работе</h2>
  <div class="case-grid">
    <div><h3>Два практических сценария</h3><p>Первый — превратить запись разговора в текст через HTTP API. Второй — находить старые решения и контекст задачи в рабочей переписке.</p></div>
    <div><h3>Что собрал</h3><p>Подготовил FastAPI-сервис на VOSK с ffmpeg, таймкодами и наблюдаемостью; для чатов — webhook-бота, полнотекстовый поиск и подключение контекста к Codex через MCP-подход.</p></div>
    <div><h3>Почему это важно</h3><p>Это не демонстрация модели ради модели: оба инструмента экономят время на рутинной работе и остаются self-hosted. <a href="https://github.com/lvipa/vosk-smart-stt-api" target="_blank" rel="noopener">STT API ↗</a> · <a href="https://github.com/lvipa/express-chat-context" target="_blank" rel="noopener">поиск контекста ↗</a></p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Краткосрочный проект · HPC · Slurm · Ceph</p>
  <h2>Подготовил вычислительный кластер к передаче в эксплуатацию</h2>
  <div class="case-grid">
    <div><h3>Контекст</h3><p>Это отдельный проект для университета, а не основное место работы. Нужно было привести кластеры в состояние, в котором ими можно безопасно пользоваться каждый день.</p></div>
    <div><h3>Что сделал</h3><p>Проверил Slurm и CephFS, настроил резервный контроллер, ограничения CPU и памяти, общую файловую систему и шаблоны для расчётов VASP и Gaussian.</p></div>
    <div><h3>Результат</h3><p>Появились рабочая очередь, проверенные тестовые расчёты и короткая инструкция по проверке состояния — без зависимости от человека, который настраивал кластер.</p></div>
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
