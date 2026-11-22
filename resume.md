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
      <p>Самара, Россия · Рассматриваю удалённую и&nbsp;гибридную работу</p>
      <p class="resume-links"><a href="mailto:lvipa@ivanlipatov.ru">E-mail</a><a href="https://t.me/lvipa">Telegram</a><a href="https://github.com/lvipa">GitHub</a><a href="https://www.linkedin.com/in/lvipa/">LinkedIn</a></p>
    </div>
    <img src="{{ '/assets/images/ivan-lipatov.jpeg' | relative_url }}" alt="Иван Липатов" class="resume-photo">
  </div>

  <section class="resume-highlights" aria-label="Основные направления">
    <div><strong>С 2017</strong><span>работаю в&nbsp;ИТ</span></div>
    <div><strong>С 2020</strong><span>в&nbsp;СМС-ИТ</span></div>
    <div><strong>CI/CD</strong><span>TeamCity и&nbsp;автоматизация сборок</span></div>
    <div><strong>Docker</strong><span>Compose и&nbsp;Kubernetes</span></div>
    <div><strong>Скрипты</strong><span>PowerShell, Bash, Python</span></div>
  </section>

  <div class="resume-layout">
    <div class="resume-main">
      <h2>Опыт работы</h2>

      <section class="resume-employer-group" aria-label="Основной опыт в&nbsp;СМС-ИТ">
        <header class="resume-employer-head">
          <p>Сентябрь 2020 — настоящее время</p>
          <h3>СМС-Информационные технологии, ООО</h3>
          <span>От внедрения систем у&nbsp;заказчиков до&nbsp;CI/CD и&nbsp;внутренней инфраструктуры</span>
        </header>

        <article class="resume-job resume-job--current">
          <h3>Ведущий специалист по&nbsp;внедрению ИС / Senior DevOps &amp; Infrastructure Engineer</h3>
          <p class="resume-meta">Февраль 2024 - н.в. · Самара, Россия</p>
          <p>Развиваю CI/CD и&nbsp;сопровождаю внутреннюю инфраструктуру компании: сборку и&nbsp;поставку приложений, тестовые среды, Linux- и&nbsp;Windows-серверы.</p>
          <ul>
            <li>Настроил и&nbsp;поддерживаю сборку, тестирование и&nbsp;деплой .NET-, Python- и&nbsp;frontend-приложений через TeamCity. Автоматизировал синхронизацию веток между deploy- и&nbsp;build-конфигурациями через REST API.</li>
            <li>Реализовал и&nbsp;проверил подписание EXE/DLL и&nbsp;установщиков в&nbsp;трёх сборочных цепочках: изменение версии, подпись, проверка и&nbsp;упаковка артефактов.</li>
            <li>Развернул GitLab Runner в&nbsp;Docker на&nbsp;Debian 12: Docker executor, приватный registry и&nbsp;образ .NET SDK.</li>
            <li>Развернул новый стенд Keycloak в&nbsp;Kubernetes. Проверил миграцию копии PostgreSQL-базы, настроил Secrets, probes, ресурсы контейнера и&nbsp;публикацию через MetalLB.</li>
            <li>Развернул Portainer через Helm с&nbsp;PV/PVC и&nbsp;HTTPS. Подключил шесть Docker-хостов без перезапуска приложений, настроил AD/LDAPS и&nbsp;сетевые ограничения для&nbsp;агентов.</li>
            <li>Настроил авторизацию тестовых сред через Keycloak/OIDC и&nbsp;ADFS: claims, группы, роли и&nbsp;проверка пользовательского входа.</li>
            <li>Для трёх AI-сервисов настроил обновление и&nbsp;откат через TeamCity с&nbsp;сохранением моделей и&nbsp;данных. Добавил проверки готовности в&nbsp;Zabbix без отправки пользовательских документов.</li>
            <li>Автоматизировал восстановление тестовых БД из&nbsp;шаблонов. Сопровождаю PostgreSQL, Redis, S3/MinIO, Nginx/IIS, резервное копирование и&nbsp;мониторинг.</li>
            <li>Разрабатывал PowerShell-инструменты запуска Trivy, Semgrep и&nbsp;CodeQL со сводными JSON/SARIF- и&nbsp;Excel-отчётами. Развёртывал VOSK/FastAPI и&nbsp;сервис транскрибации.</li>
          </ul>
          <p><a href="{{ '/projects/' | relative_url }}">Подробности реализаций и&nbsp;открытые примеры →</a></p>
          <div class="resume-project-note">
            <h4>Дополнительный проектный опыт · март — июнь 2026</h4>
            <p>Параллельно основной работе ввёл в&nbsp;эксплуатацию три HPC-кластера по&nbsp;10 серверов для&nbsp;Самарского государственного технического университета: Linux, Slurm, Ceph/CephFS, сеть на&nbsp;SONiC. Настраивал хранилище и&nbsp;очереди заданий, разбирал аппаратные и&nbsp;сетевые сбои, подготовил документацию.</p>
          </div>
        </article>

        <article class="resume-job">
          <h3>Старший специалист службы внедрения</h3>
          <p class="resume-meta">Декабрь 2021 - Январь 2024 · Самара, Россия</p>
          <ul>
            <li>Внедрял и&nbsp;сопровождал корпоративную систему для&nbsp;крупных заказчиков: Windows/Debian, IIS, .NET Core, PostgreSQL, Redis Cluster, Docker, Ceph и&nbsp;MinIO/S3.</li>
            <li>Разобрал инцидент с&nbsp;деградацией системы на&nbsp;нескольких контурах: проверил приложение, ОС, сеть, reverse proxy, БД и&nbsp;CI/CD. Устранил причины и&nbsp;привёл конфигурации к&nbsp;единому виду.</li>
            <li>Согласовывал технические решения с&nbsp;ИБ и&nbsp;командами заказчиков, участвовал в&nbsp;автоматизации деплоя, настройке мониторинга и&nbsp;резервного копирования.</li>
          </ul>
        </article>

        <article class="resume-job">
          <h3>Специалист службы внедрения</h3>
          <p class="resume-meta">Сентябрь 2020 - Ноябрь 2021 · Самара, Россия</p>
          <ul>
            <li>Подготавливал тестовые и&nbsp;серверные площадки для&nbsp;SCADA и&nbsp;аналитических систем; проводил нагрузочное и&nbsp;стресс-тестирование, анализировал метрики и&nbsp;участвовал в&nbsp;устранении узких мест.</li>
            <li>Администрировал Windows Server и&nbsp;PostgreSQL, участвовал в&nbsp;настройке Docker, Ceph, MinIO, S3-хранилищ, мониторинга и&nbsp;резервного копирования.</li>
          </ul>
        </article>
      </section>

      <article class="resume-job">
        <h3>Специалист внедрения и&nbsp;технической поддержки</h3>
        <p class="resume-company">ИнфоПро, группа компаний</p>
        <p class="resume-meta">Сентябрь 2017 - Август 2019 · Самара, Россия</p>
        <ul><li>Внедрял ПО для&nbsp;энергетической отрасли: настраивал расчётные сценарии, алгоритмы и&nbsp;отчётность.</li><li>Автоматизировал сбор и&nbsp;обработку данных на&nbsp;C#, включая HTTP-запросы и&nbsp;обработку файлов. Работал с&nbsp;SQL, PostgreSQL и&nbsp;MS SQL Server.</li><li>Разбирал ошибки, тестировал функциональность, готовил инструкции и&nbsp;консультировал пользователей.</li></ul>
      </article>
    </div>

    <aside class="resume-side">
      <h2>Образование</h2>
      <p><strong>Самарский государственный технический университет</strong><br>Высшее образование, математическое обеспечение и&nbsp;администрирование информационных систем<br>2017</p>
      <h2>Навыки</h2>
      <p><strong>CI/CD:</strong> TeamCity, GitLab Runner, REST API, Git</p>
      <p><strong>Контейнеры:</strong> Docker, Docker Compose, Kubernetes, Helm, Portainer</p>
      <p><strong>Системы и&nbsp;скрипты:</strong> Linux, Windows Server, Bash, PowerShell, Python, systemd</p>
      <p><strong>Данные:</strong> PostgreSQL, Redis, S3/MinIO, Ceph/CephFS</p>
      <p><strong>Мониторинг:</strong> Zabbix, Grafana, ELK, Graylog</p>
      <p><strong>Сеть и&nbsp;доступ:</strong> Nginx, IIS, DNS, TLS, AD, GPO, Keycloak, OIDC, ADFS</p>
      <p><strong>Анализ безопасности:</strong> Trivy, Semgrep, CodeQL</p>
      <p><strong>Базовый опыт:</strong> Ansible — тестовые задачи</p>
      <h2>Языки</h2>
      <p>Русский — родной<br>Английский — B1 (Intermediate)</p>
      <h2>Скачать PDF</h2>
      <p class="resume-downloads"><a class="button button-primary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_RU.pdf' | relative_url }}">Русская версия</a><a class="button button-secondary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_EN.pdf' | relative_url }}">English version</a></p>
    </aside>
  </div>
</section>
