# Steam Card Farmer 0.13.4-dev — Android 14–16 return test

## RU

Тестовая сборка для автоматического возврата в Card Farmer после подтверждения входа в Steam Mobile.

Важно: Card Farmer не пытается закрывать или «сворачивать» Steam. Вместо этого после выдачи итоговой Steam-сессии приложение использует штатный Android PendingIntent с разрешённым background activity start и поднимает собственный task на передний план. Это соответствует ограничениям Android 14–16.

Если прошивка всё равно запрещает автоматический возврат, остаётся приватное уведомление с переходом назад в Card Farmer.

## EN

Test build for returning to Card Farmer after Steam Mobile approval on Android 14–16.

Card Farmer does not attempt to close or minimize Steam. After Steam issues the final session, it uses the Android-supported PendingIntent background-activity-start opt-in to bring its own task to the foreground. A private notification remains as fallback.

Source commit: c6f15742d380c5112d991c1344b95f4d4f558fb5
APK SHA-256: 80e55ca9169d7e8a31e89b38e47fc0aef8c06192cf75025a93c3ed775a9e8d5d
