# Steam Card Farmer 0.13.3-dev — Return after Steam approval test

## RU

Тестовая сборка исправляет возврат после одобрения входа в Steam Mobile.

После выдачи итоговой Steam-сессии Card Farmer пытается автоматически вернуть свой Android task на передний план. Если Android или прошивка Samsung блокирует автоматический возврат, появляется приватное системное уведомление «Вход в Steam подтверждён» с кнопкой-переходом обратно в Card Farmer.

Также сохраняются исправления polling и восстановления ожидающей auth-сессии из 0.13.2-dev.

## EN

Test build for returning to Card Farmer after Steam Mobile approves the sign-in.

After Steam issues the final session, Card Farmer attempts to bring its Android task back to the foreground. If Android/OEM policy blocks automatic foregrounding, a private system notification provides a one-tap return path.

Source commit: e95f78fe3b0860bb90c574ba5c7597c9675a2aa9
APK SHA-256: b23b64577204f1fa67a4fc4c100de71976ee3fb6ba62a38afe3fe4e78720584d
