# Steam Card Farmer 0.13.2-dev — Approved-session completion test

## RU

Тестовая сборка для исправления ситуации, когда Steam Mobile уже показывает «Запрос на вход одобрен», а Card Farmer не получает итоговую Steam-сессию.

Исправлено:
- обработка смены client_id при polling Steam;
- повтор polling после временных сетевых ошибок;
- немедленная повторная проверка после возврата из Steam Mobile;
- зашифрованное сохранение ожидающей auth-сессии и восстановление после пересоздания/убийства Activity;
- синхронная запись защищённых токенов/ожидающей сессии в локальное защищённое хранилище.

Пароль и код Steam Guard не сохраняются и не должны отправляться кому-либо.

## EN

Test build for the case where Steam Mobile already reports that the login request was approved but Card Farmer does not receive the final Steam session.

Fixed:
- client_id rotation handling during Steam polling;
- polling retries after transient network errors;
- immediate re-check after returning from Steam Mobile;
- encrypted pending-auth persistence and restoration after Activity/process recreation;
- synchronous persistence of protected session state.

Source commit: 746c3425c24093472d69b9b8bae1f5d8b0a843fa
APK SHA-256: 324f8acd38cdb768f7cc66aeceabacd04c6fa442d950ca3217925ea9e282c5f5
