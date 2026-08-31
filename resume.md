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

  <section class="resume-highlights" aria-label="Ключевые результаты">
    <div><strong>50+</strong><span>сервисов в TeamCity CI/CD</span></div>
    <div><strong>30+</strong><span>Linux- и Windows-серверов</span></div>
    <div><strong>50–70%</strong><span>меньше ручных операций</span></div>
    <div><strong>6 лет</strong><span>непрерывного опыта в СМС-ИТ</span></div>
  </section>

  <div class="resume-layout">
    <div class="resume-main">
      <h2>Опыт работы</h2>

      <section class="resume-employer-group" aria-label="Основной опыт в СМС-ИТ">
        <header class="resume-employer-head">
          <p>Основной опыт · Сентябрь 2020 - н.в.</p>
          <h3>СМС-Информационные технологии, ООО</h3>
          <span>Рост от специалиста службы внедрения до Senior DevOps &amp; Infrastructure Engineer</span>
        </header>

        <article class="resume-job resume-job--current">
          <h3>Senior DevOps &amp; Infrastructure Engineer</h3>
          <p class="resume-meta">Февраль 2024 - н.в. · Самара, Россия</p>
          <ul>
            <li>Развил и стандартизировал TeamCity CI/CD для 50+ сервисов: сборка, тестирование, публикация артефактов и деплой .NET- и frontend-приложений в Linux- и Windows-окружения.</li>
            <li>Перевёл очистку и ротацию файлов, проверки сервисов и БД, а также сбор диагностики в сценарии PowerShell, Bash и Python; ручное участие снизилось на 50–70%.</li>
            <li>Стандартизировал окружения, структуру каталогов, логирование и health-check'и: релизные операции стали в 2–3 раза быстрее и устойчивее.</li>
            <li>Сопровождаю 30+ Linux- и Windows-серверов, Docker, PostgreSQL и S3/MinIO; настраиваю Nginx/IIS reverse proxy, резервное копирование и наблюдаемость через Zabbix, Grafana, ELK и Graylog.</li>
          </ul>
        </article>

        <article class="resume-job">
          <h3>Старший специалист службы внедрения</h3>
          <p class="resume-meta">Декабрь 2021 - Январь 2024 · Самара, Россия</p>
          <ul>
            <li>Решил сложный инцидент с деградацией корпоративной системы на нескольких контурах: диагностировал цепочку от приложения до БД и CI/CD, устранил причины и стандартизировал конфигурации.</li>
            <li>Внедрял и сопровождал enterprise-систему для крупных заказчиков: Windows/Debian, IIS, .NET Core, PostgreSQL, Redis Cluster, Docker, Ceph, MinIO и S3.</li>
          </ul>
        </article>

        <article class="resume-job">
          <h3>Специалист службы внедрения</h3>
          <p class="resume-meta">Сентябрь 2020 - Ноябрь 2021 · Самара, Россия</p>
          <ul>
            <li>Подготавливал тестовые и серверные площадки для SCADA и аналитических систем; проводил нагрузочное и стресс-тестирование, анализировал метрики и устранял узкие места.</li>
            <li>Администрировал Windows Server и PostgreSQL, участвовал в настройке Docker, Ceph, MinIO, S3-хранилищ, мониторинга и резервного копирования.</li>
          </ul>
        </article>
      </section>

      <article class="resume-job">
        <h3>Дополнительный проект: Infrastructure / DevOps Engineer - HPC</h3>
        <p class="resume-company">Самарский государственный технический университет</p>
        <p class="resume-meta">Март 2026 - Июнь 2026 · Параллельный проект</p>
        <ul>
          <li>Ввёл в эксплуатацию три HPC-кластера по 10 серверов для инженерных и научных расчётов.</li>
          <li>Развернул Ceph и Slurm, настроил SONiC, VLAN и MTU; работал с IPMI, iDRAC, BMC и Redfish API.</li>
        </ul>
      </article>

      <article class="resume-job">
        <h3>Специалист внедрения и технической поддержки</h3>
        <p class="resume-company">ИнфоПро, группа компаний</p>
        <p class="resume-meta">Сентябрь 2017 - Август 2019 · Самара, Россия</p>
        <ul><li>Внедрение ПО для энергетической отрасли, автоматизация сбора данных и работа с SQL, PostgreSQL и MS SQL Server.</li></ul>
      </article>
    </div>

    <aside class="resume-side">
      <h2>Образование</h2>
      <p><strong>Самарский государственный технический университет</strong><br>Высшее образование, математическое обеспечение и администрирование информационных систем<br>2017</p>
      <h2>Навыки</h2>
      <p><strong>CI/CD и автоматизация:</strong> TeamCity, Docker, Docker Compose, Bash, PowerShell, Python<br><strong>Платформы:</strong> Linux, Windows Server, AD, DNS, GPO, IIS<br><strong>Данные и хранение:</strong> PostgreSQL, Redis, S3/MinIO, Ceph<br><strong>Наблюдаемость и сеть:</strong> Nginx, Zabbix, Grafana, ELK, Graylog, Slurm, SONiC, IPMI/iDRAC</p>
      <h2>Языки</h2>
      <p>Русский — родной<br>Английский — B1 (Intermediate)</p>
      <h2>Скачать PDF</h2>
      <p class="resume-downloads"><a class="button button-primary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_RU.pdf' | relative_url }}">Русская версия</a><a class="button button-secondary" href="{{ '/assets/resume/Ivan_Lipatov_Senior_DevOps_Infrastructure_Engineer_EN.pdf' | relative_url }}">English version</a></p>
    </aside>
  </div>
</section>
