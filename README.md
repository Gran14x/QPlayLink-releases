# QPlayLink

Вся игровая статистика в одном окне — для Windows 10/11.

**🌐 Страница программы: [gran14x.github.io/QPlayLink-releases](https://gran14x.github.io/QPlayLink-releases/)** — скриншоты, видео и кнопка «Скачать».

Вводите ник, ссылку на Steam или Riot ID — и видите рейтинг, историю матчей, героев и прогресс.
Свои профили и друзей можно добавить в избранное и следить за ростом рейтинга.

## Скачать

**[Последняя версия → Releases](../../releases/latest)**

1. Скачайте **`QPlayLink-Setup-<версия>.exe`** и запустите.
2. Нажмите «Установить» — права администратора не нужны, ярлыки появятся в «Пуске» и (по желанию) на рабочем столе.
3. Дальше программа обновляется сама — скачиваются только изменившиеся файлы.

Удаление — как у обычной программы: «Параметры → Приложения → QPlayLink → Удалить».

Без установки: скачайте `QPlayLink-<версия>.zip`, распакуйте в любую папку и запустите `QPlayLink.exe`
(папка `_internal` рядом нужна программе — не удаляйте её).

> Windows SmartScreen может предупредить о неизвестном издателе — нажмите «Подробнее» → «Выполнить в любом случае».
> У программы нет платной цифровой подписи.

## Игры

| Игра | Что показывает | Источник |
|---|---|---|
| Dota 2 | Матчи, герои, форма, разбор матча, контрпики | OpenDota |
| Counter-Strike 2 | Premier-рейтинг, ранги по картам, последние матчи | Leetify |
| FACEIT | ELO, уровень, карты, K/D, последние матчи | официальный API FACEIT |
| League of Legends | Ранг, LP, мастерство чемпионов, последние матчи | официальный API Riot Games |
| Deadlock | Ранг, герои, последние матчи | deadlock-api.com |
| Overwatch 2 | Ранги по ролям, контрпики | OverFast API |
| Apex Legends | Ранг, RP, легенды | Apex Legends Status |
| War Thunder | Эффективность по режимам и технике | ThunderSkill |
| Chess.com | Рейтинг по режимам, партии | официальный API Chess.com |
| Steam | Уровень, библиотека, часы в играх | официальный API Steam |
| Brawl Stars | Кубки, бойцы, бои | официальный API Supercell |
| Genshin Impact · Honkai: Star Rail · Zenless Zone Zero | Витрина персонажей, достижения | Enka.Network |

**Скоро:** Valorant — вернётся со входом через аккаунт Riot (так требуют правила Riot Games);
Мир Танков — после подключения официального API Lesta.

## Возможности

- **История рейтинга и цели** — график за месяц/год, пик и минимум, уведомление при достижении цели.
- **Избранное и группы друзей** — общая таблица рейтинга, видно, кто вырос за неделю.
- **«Друг зашёл в игру»** — уведомления в программе и в Telegram.
- **Мини-окно поверх игр** и **автооткрытие раздела** при запуске игры.
- **Публичная страница профиля** — своя статистика по ссылке, открывается с телефона.
- Тёмная и светлая темы, русский и английский интерфейс.

## Данные и безопасность

- Программа **не читает память игр и не меняет их файлы** — только открытые данные игровых сервисов. Античит она не затрагивает.
- Пароли от Steam и других сервисов не нужны и не запрашиваются. Steam привязывается через официальный вход Steam.
- Ключи API игровых сервисов хранятся только на сервере QPlayLink — в программе их нет.
- Нужен бесплатный аккаунт QPlayLink: ник и пароль или вход через Steam/Discord. Почта необязательна — только для восстановления пароля.
- Ваши данные не продаются и не передаются третьим лицам.

## Обратная связь

Ошибки и предложения — Telegram-боту [@QPlayLink_bot](https://t.me/QPlayLink_bot), в программе («Настройки → Сообщить о проблеме»)
или во вкладке [Issues](../../issues). Ответ разработчика придёт туда же.
Если программа упадёт, описание ошибки уйдёт разработчику само (это можно выключить в настройках).

## Лицензия

**QPlayLink** — бесплатная программа с закрытым исходным кодом. © 2026 Greno4ka. Все права защищены.
Использование — на условиях [LICENSE](LICENSE) и лицензионного соглашения, которое показывается при первом запуске программы.

В программу входят открытые сторонние компоненты, каждый — под своей лицензией:

| Компонент | Лицензия |
|---|---|
| Qt 6, PySide6, Shiboken6 | GNU LGPL v3 |
| Python и встроенные в него библиотеки (OpenSSL, SQLite, zlib, expat, libffi и др.) | PSF License, Apache 2.0, MIT, BSD, zlib |
| requests, packaging | Apache 2.0 |
| urllib3, charset-normalizer, curl_cffi, cffi, setuptools | MIT |
| idna, pycparser | BSD-3-Clause |
| certifi | MPL 2.0 |
| curl, BoringSSL, nghttp2, Brotli, Zstandard (внутри curl_cffi) | curl, Apache 2.0, MIT, BSD |

Qt и PySide6 используются без изменений и лежат отдельными библиотеками в папке `_internal\PySide6` — их можно заменить своей совместимой сборкой.
Исходный код Qt: [download.qt.io](https://download.qt.io/official_releases/qt/), PySide6: [Qt for Python](https://download.qt.io/official_releases/QtForPython/).

Полные тексты всех лицензий — в файле [THIRD_PARTY_LICENSES.txt](THIRD_PARTY_LICENSES.txt) и в программе:
Настройки → Система → О программе → «Лицензии».

QPlayLink не связан с Valve, Riot Games, Blizzard, EA, Gaijin, Supercell, HoYoverse, FACEIT и Chess.com.
Названия игр и логотипы принадлежат их владельцам.

QPlayLink isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.

This material is unofficial and is not endorsed by Supercell. For more information see Supercell's Fan Content Policy: www.supercell.com/fan-content-policy.
