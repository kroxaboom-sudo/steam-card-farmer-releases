# Steam Card Farmer 0.13.5-dev — Card discovery redirect fix

## RU

Тестовая сборка исправляет поиск игр с оставшимися карточками.

Причина: Steam Community перенаправляет числовой профиль /profiles/<steamid>/... на vanity-профиль /id/<name>/..., а Card Farmer намеренно запрещал автоматические HTTP-redirect и воспринимал корректный ответ Steam как ошибку.

Теперь переходы обрабатываются вручную, максимум 5 шагов, только по HTTPS и только внутри steamcommunity.com. Авторизационные cookies сохраняются между разрешёнными переходами.

Также добавлена диагностика неудачного card-drop scan в общий observability-контур.

## EN

Test build fixing discovery of games with remaining Steam card drops.

Steam Community can redirect numeric /profiles/<steamid>/ URLs to vanity /id/<name>/ URLs. Card Farmer previously treated that legitimate redirect as an error. Redirects are now handled explicitly with a strict HTTPS + steamcommunity.com allowlist and a five-hop limit.

Source commit: eed59789f41fa093457b98d715f52224782e50b8
APK SHA-256: 2d9d031c746677107e1cc3c713ca0d11a04450bd532b3fdf5a1e2a09cb23b9f9
