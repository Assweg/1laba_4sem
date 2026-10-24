# Интерфейс мониторинга энергообъектов

![Стек](https://img.shields.io/badge/React%2018%20%C2%B7%20Chart.js-334155?style=flat-square) ![Семестр](https://img.shields.io/badge/семестр-4-0f766e?style=flat-square) ![Статус](https://img.shields.io/badge/статус-%D0%A3%D1%87%D0%B5%D0%B1%D0%BD%D1%8B%D0%B9%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82-64748b?style=flat-square)

Лабораторная №1: React-интерфейс системы мониторинга с маршрутизацией, запросами через Axios и графиками Chart.js. Для локальных данных предусмотрен JSON Server.

## Файлы

- [src](src/) — страницы, компоненты и стили.
- [public](public/) — статические ресурсы.
- [db.json](db.json) — данные для локального API.
- [package.json](package.json) — зависимости и команды.

## Локальный запуск

Нужен Node.js с npm. Установка зависимостей и запуск интерфейса:

```bash
npm ci
npm start
```

В другом терминале запустите API. Скрипт `npm run server` использует `json-server`, но пакет не объявлен в зависимостях, поэтому для запуска без изменения проекта можно явно выбрать совместимую версию:

```bash
npx --yes json-server@0.17.4 --watch db.json --port 7431
```

Интерфейс CRA обычно открывается на `http://localhost:3000`, API — на `http://localhost:7431`.

## Сборка

```bash
npm run build
```

## Продолжение

[Полная система с backend и БД](https://github.com/Assweg/4laba_4sem).

---

[Все учебные работы](https://github.com/Assweg/nstu) · [Профиль Assweg](https://github.com/Assweg)
