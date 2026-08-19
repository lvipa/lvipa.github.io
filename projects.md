---
layout: default
title: Проекты
permalink: /projects/
lang: ru
translation: /en/projects/
---

# Проекты

<p class="page-intro">Обезличенная выборка инфраструктурных и DevOps-проектов: от устойчивости кластеров до CI/CD, тестовых сред и инженерных quality gates.</p>

<section class="case-study">
  <p class="case-kicker">CI/CD · Security</p>
  <h2>Security scanning как часть сборки</h2>
  <div class="case-grid">
    <div><h3>Задача</h3><p>Получать ранний сигнал об уязвимостях зависимостей и проблемах в коде, не дожидаясь внешнего аудита.</p></div>
    <div><h3>Решение</h3><p>Собрал сценарии SCA/SAST с Trivy, Semgrep, CodeQL и проверкой зависимостей. Добавил targeted-запуск по solution, отдельные каталоги отчётов и исключения generated-файлов.</p></div>
    <div><h3>Результат</h3><p>Единый воспроизводимый контур для frontend, backend и legacy-кода без смешивания результатов разных запусков.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">PostgreSQL · HA · Compliance</p>
  <h2>Контроль дрейфа конфигурации HA-кластера</h2>
  <div class="case-grid">
    <div><h3>Задача</h3><p>Снизить риск отличий между эталонной и фактической конфигурацией кластера PostgreSQL.</p></div>
    <div><h3>Решение</h3><p>Автоматизировал сравнение конфигураций etcd, Patroni, HAProxy и Keepalived с учётом runtime-параметров PostgreSQL, комментариев и окруженческих значений.</p></div>
    <div><h3>Результат</h3><p>Проверка стала понятным техническим аудитом: отклонения видны до того, как превратятся в инцидент.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Linux · TeamCity · Testing</p>
  <h2>Миграция тестовых площадок на Linux</h2>
  <div class="case-grid">
    <div><h3>Задача</h3><p>Перенести площадки и автотесты на единый Linux-контур без потери воспроизводимости.</p></div>
    <div><h3>Решение</h3><p>Подготовил systemd-сервисы, Docker-развёртывание, PostgreSQL-конфигурацию и порядок pipeline: restore БД → deploy → UI-тесты → API-тесты.</p></div>
    <div><h3>Результат</h3><p>Тестовая среда стала ближе к production-подходу и проще для повторного запуска и диагностики.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">Release engineering · Quality gate</p>
  <h2>Контроль состава артефактов</h2>
  <div class="case-grid">
    <div><h3>Задача</h3><p>Замечать неожиданные файлы в новых артефактах до передачи релиза.</p></div>
    <div><h3>Решение</h3><p>Выделил отдельную проверку в CI, сравнивающую состав текущего и референсного артефакта, включая вложенные ZIP-архивы.</p></div>
    <div><h3>Результат</h3><p>Команда получает diff и уведомление, а основной build остаётся независимым от процесса ревизии.</p></div>
  </div>
</section>

<section class="case-study">
  <p class="case-kicker">SonarQube · Build agents</p>
  <h2>Переносимый анализ качества кода</h2>
  <div class="case-grid">
    <div><h3>Задача</h3><p>Запускать анализ C# на разных build-агентах, несмотря на различия в окружении.</p></div>
    <div><h3>Решение</h3><p>Стандартизировал JDK и scanner-инструменты, настройку переменных среды, доверие к сертификатам и лимиты reverse proxy для крупных отчётов.</p></div>
    <div><h3>Результат</h3><p>Качество кода проверяется не на «особом» агенте, а как обычная часть CI-процесса.</p></div>
  </div>
</section>

<p class="page-note">Все примеры намеренно обезличены: без названий компаний, адресов, учётных данных и внутренних схем.</p>
