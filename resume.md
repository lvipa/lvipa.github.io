---
layout: default
title: Резюме - Иван Липатов
description: Senior DevOps / Infrastructure Engineer - опыт, навыки и версии резюме.
permalink: /resume/
lang: ru
translation: /en/resume/
---

<section class="resume-page shell">
  <div class="resume-head">
    <div>
      <p class="resume-kicker">Senior DevOps &amp; Infrastructure Engineer</p>
      <h1>Иван Липатов</h1>
      <p>Самара, Россия · Рассматриваю удалённую и гибридную работу</p>
      <p class="resume-links"><a href="mailto:lvipa@ivanlipatov.ru">E-mail</a><a href="https://t.me/lvipa">Telegram</a><a href="https://github.com/lvipa">GitHub</a><a href="https://www.linkedin.com/in/lvipa/">LinkedIn</a></p>
    </div>
    <img src="{{ '/assets/images/ivan-lipatov.jpeg' | relative_url }}" alt="Иван Липатов" class="resume-photo">
  </div>

  <section class="resume-highlights" aria-label="Основные направления">
    <div><strong>С 2017</strong><span>работаю в ИТ</span></div>
    <div><strong>С 2020</strong><span>в СМС-ИТ</span></div>
    <div><strong>CI/CD</strong><span>TeamCity и автоматизация сборок</span></div>
    <div><strong>Docker</strong><span>Compose и Kubernetes</span></div>
    <div><strong>Скрипты</strong><span>PowerShell, Bash, Python</span></div>
  </section>

  <div class="resume-layout">
    <div class="resume-main">
      <h2>Опыт работы</h2>

      <section class="resume-employer-group" aria-label="Основной опыт в СМС-ИТ">
        <header class="resume-employer-head">
          <p>Сентябрь 2020 — настоящее время</p>
          <h3>СМС-Информационные технологии, ООО</h3>
          <span>От внедрения систем у заказчиков до CI/CD и внутренней инфраструктуры</span>
        </header>

        <article class="resume-job resume-job--current">
          <h3>Ведущий специалист по внедрению ИС / Senior DevOps &amp; Infrastructure Engineer</h3>
          <p class="resume-meta">Февраль 2024 - н.в. · Самара, Россия</p>
          <p>Развиваю CI/CD и сопровождаю внутреннюю инфраструктуру компании: сборку и поставку приложений, тестовые среды, Linux- и Windows-серверы.</p>
          <ul>
            <li>Настроил и поддерживаю сборку, тестирование и деплой .NET-, Python- и frontend-приложений через TeamCity. Автоматизировал синхронизацию веток между deploy- и build-конфигурациями через REST API.</li>
            <li>Реализовал и проверил подписание EXE/DLL и установщиков в трёх сборочных цепочках: изменение версии, подпись, проверка и упаковка артефактов.</li>
            <li>Развернул GitLab Runner в Docker на Debian 12: Docker executor, приватный registry и образ .NET SDK.</li>
            <li>Развернул новый стенд Keycloak в Kubernetes. Проверил миграцию копии PostgreSQL-базы, настроил Secrets, probes, ресурсы контейнера и публикацию через MetalLB.</li>
            <li>Развернул Portainer через Helm с PV/PVC и HTTPS. Подключил шесть Docker-хостов без перезапуска приложений, настроил AD/LDAPS и сетевые ограничения для агентов.</li>
            <li>Настроил авторизацию тестовых сред через Keycloak/OIDC и ADFS: claims, группы, роли и проверка пользовательского входа.</li>
            <li>Для трёх AI-сервисов настроил обновление и откат через TeamCity с сохранением моделей и данных. Добавил проверки готовности в Zabbix без отправки пользовательских документов.</li>
            <li>Автоматизировал восстановление тестовых БД из шаблонов. Сопровождаю PostgreSQL, Redis, S3/MinIO, Nginx/IIS, резервное копирование и мониторинг.</li>
            <li>Разрабатывал PowerShell-инструменты запуска Trivy, Semgrep и CodeQL со сводными JSON/SARIF- и Excel-отчётами. Развёртывал VOSK/FastAPI и сервис транскрибации.</li>
          </ul>
          <p><a href="{{ '/projects/' | relative_url }}">Подробности реализаций и открытые примеры →</a></p>
          <div class="resume-project-note">
            <h4>Дополнительный проектный опыт · март — июнь 2026</h4>
            <p>Параллельно основной работе ввёл в эксплуатацию три HPC-кластера по 10 серверов для Самарского государственного технического университета: Linux, Slurm, Ceph/CephFS, сеть на SONiC. Настраивал хранилище и очереди заданий, разбирал аппаратные и сетевые сбои, подготовил документацию.</p>
          </div>
        </article>

        <article class="resume-job">
          <h3>Старший специалист службы внедрения</h3>
          <p class="resume-meta">Декабрь 2021 - Январь 2024 · Самара, Россия</p>
          <ul>
            <li>Внедрял и сопровождал корпоративную систему для крупных заказчиков: Windows/Debian, IIS, .NET Core, PostgreSQL, Redis Cluster, Docker, Ceph и MinIO/S3.</li>
            <li>Разобрал инцидент с деградацией системы на нескольких контурах: проверил приложение, ОС, сеть, reverse proxy, БД и CI/CD. Устранил причины и привёл конфигурации к единому виду.</li>
            <li>Согласовывал технические решения с ИБ и командами заказчиков, участвовал в автоматизации деплоя, настройке мониторинга и резервного копирования.</li>
          </ul>
        </article>

        <article class="resume-job">
          <h3>Специалист службы внедрения</h3>
          <p class="resume-meta">Сентябрь 2020 - Ноябрь 2021 · Самара, Россия</p>
          <ul>
            <li>Подготавливал тестовые и серверные площадки для SCADA и аналитических систем; проводил нагрузочное и стресс-тестирование, анализировал метрики и участвовал в устранении узких мест.</li>
            <li>Администрировал Windows Server и PostgreSQL, участвовал в настройке Docker, Ceph, MinIO, S3-хранилищ, мониторинга и резервного копирования.</li>
          </ul>
        </article>
      </section>

      <article class="resume-job">
        <h3>Специалист внедрения и технической поддержки</h3>
        <p class="resume-company">ИнфоПро, группа компаний</p>
        <p class="resume-meta">Сентябрь 2017 - Август 2019 · Самара, Россия</p>
        <ul><li>Внедрял ПО для энергетической отрасли: настраивал расчётные сценарии, алгоритмы и отчётность.</li><li>Автоматизировал сбор и обработку данных на C#, включая HTTP-запросы и обработку файлов. Работал с SQL, PostgreSQL и MS SQL Server.</li><li>Разбирал ошибки, тестировал функциональность, готовил инструкции и консультировал пользователей.</li></ul>
      </article>
    </div>

    <aside class="resume-side">
      <h2>Образование</h2>
      <p><strong>Самарский государственный технический университет</strong><br>Высшее образование, математическое обеспечение и администрирование информационных систем<br>2017</p>
      <h2>Навыки</h2>
      <p><strong>CI/CD:</strong> TeamCity, GitLab Runner, REST API, Git</p>
      <p><strong>Контейнеры:</strong> Docker, Docker Compose, Kubernetes, Helm, Portainer</p>
      <p><strong>Системы и скрипты:</strong> Linux, Windows Server, Bash, PowerShell, Python, systemd</p>
      <p><strong>Данные:</strong> PostgreSQL, Redis, S3/MinIO, Ceph/CephFS</p>
      <p><strong>Мониторинг:</strong> Zabbix, Grafana, ELK, Graylog</p>
      <p><strong>Сеть и доступ:</strong> Nginx, IIS, DNS, TLS, AD, GPO, Keycloak, OIDC, ADFS</p>
      <p><strong>Анализ безопасности:</strong> Trivy, Semgrep, CodeQL</p>
      <p><strong>Базовый опыт:</strong> Ansible — тестовые задачи</p>
      <h2>Языки</h2>
      <p>Русский — родной<br>Английский — B1 (Intermediate)</p>
      <h2>Скачать PDF</h2>
      <p class="resume-downloads"><a class="button button-primary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_RU.pdf' | relative_url }}">Русская версия</a><a class="button button-secondary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_EN.pdf' | relative_url }}">English version</a></p>
    </aside>
  </div>
</section>
