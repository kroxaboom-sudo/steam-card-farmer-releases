# Steam Card Farmer 0.13.1-dev — Same-device Steam Guard test

## RU

Тестовая сборка для проверки исправленной авторизации на одном устройстве.

QR-вход больше не используется как основной сценарий на том же телефоне. Приложение запускает нативную сессию Steam, пароль существует только в кратковременной памяти, шифруется текущим RSA-ключом Steam и не сохраняется. После ответа Steam используется Steam Guard: подтверждение в Steam Mobile или код Guard, который предлагает Steam.

Пароль, код Steam Guard и другие данные аккаунта не нужно отправлять разработчику или в чат.

## EN

Test build for the corrected same-device Steam authentication flow.

QR sign-in is no longer used as the primary same-device path. The app starts a native Steam authentication session; the password exists only in short-lived memory, is encrypted with Steam's current RSA key and is never stored. Steam Guard is then used according to Steam's returned confirmation policy: Steam Mobile approval or a Guard code.

Source commit: 5d519aa16cb9c829f94dd98ff3a23c07fc2421db
APK SHA-256: f7b86bc6a8dee64687394a36feab7c91641628a4b6919dd2e48c75029e6e7874
