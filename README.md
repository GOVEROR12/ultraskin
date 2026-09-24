# Ultra Skin — сторінка запису

Одна сторінка: ім’я, телефон, заявка приходить у Telegram. Текст і колір — під [Instagram Ultra Skin](https://www.instagram.com/ultraskin.cosmetology/).

## Підключити Telegram

1. У Telegram відкрийте [@BotFather](https://t.me/BotFather), надішліть `/newbot` і скопіюйте токен.
2. Напишіть цьому боту будь-яке повідомлення (або додайте його в групу адміністраторів).
3. Відкрийте в браузері `https://api.telegram.org/botВАШ_ТОКЕН/getUpdates` і знайдіть `"chat":{"id": ...}`.
4. Вставте токен і chat id у `index.html`, блок `TELEGRAM`.
5. Завантажте оновлений файл на GitHub.

Токен лежить у відкритому коді сторінки. Зробіть окремого бота тільки для заявок і не давайте йому прав в інших чатах.

## Безкоштовно на GitHub

GitHub Pages безкоштовний для **публічного** репозиторію. Сам домен у реєстратора оплачується окремо, прив’язка до GitHub — безкоштовна, сертифікат HTTPS теж.

1. Створіть публічний репозиторій, наприклад `ultraskin`.
2. Завантажте туди `index.html` (і цей README, якщо хочете).
3. **Settings → Pages → Build and deployment → Deploy from a branch**.
4. Branch: `main`, folder: `/ (root)` → Save.
5. За кілька хвилин сайт відкриється за адресою `https://ВАШ_ЛОГІН.github.io/ultraskin/`.

## Свій домен

У **Settings → Pages → Custom domain** впишіть домен, наприклад `ultraskin.ua`. GitHub створить файл `CNAME`.

У реєстратора домену додайте записи:

**Якщо сайт на `www`** (простіше):

| Тип | Ім’я | Значення |
| --- | --- | --- |
| CNAME | www | `ВАШ_ЛОГІН.github.io` |

**Якщо сайт на голому домені** (`ultraskin.ua` без www), чотири A-записи на `@`:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Після того як DNS оновиться, увімкніть **Enforce HTTPS**. Сертифікат іноді з’являється до 24 годин.

Офіційна інструкція: [Managing a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).
