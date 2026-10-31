# Kavelle: a premium interior design and architecture studio site with a Formgong form

**Live demo:** https://kavelle.formgong.com · Download: the [latest release](https://github.com/formgong/kavelle-template/releases/latest) zip.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/formgong/kavelle-template) [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fformgong%2Fkavelle-template&project-name=kavelle&repository-name=kavelle)

Each button copies the site to your GitHub and publishes it. Then replace `fk_your_access_key` in `index.html` of your copy with your Formgong access key (free at https://formgong.com/new) and commit: the host republishes on its own.

Сайт преміальної студії дизайну інтер'єру та архітектури з формою Формгонг

A dark, one-page site for an interior design or architecture studio, in a single `index.html` plus an `img/` folder. The demo studio, Kavelle, its founder, projects and numbers are fictional.

- **Header.** The wordmark in the middle, the menu on both sides, and the language on the right. It is transparent over the slider and turns solid once you scroll. On phones it becomes a menu button.
- **Project slider.** Five full-screen projects that cross-fade every 5 seconds with a slow zoom. Each title rises letter by letter above a "View project" button. Thin progress bars, a counter and arrows sit at the bottom.
- **Projects.** Three category photos (Private, Architecture, Commercial) in a row that you can drag or scroll sideways.
- **Studio philosophy.** The founder's portrait slides in from the left and the text from the right.
- **Services.** Four cards with a light top, a title and an arrow, above a photo. On hover the top turns green and the photo zooms. A click fills in the topic of the form.
- **Numbers.** Four studio figures that count up.
- **Contact.** A light section with two lines of large text running in opposite directions, and a form with floating labels and a choice of topic.
- **Footer.** Links, social icons, hours, phone and email.

Blocks fade in from their side as they scroll into view. With `prefers-reduced-motion: reduce` the slider stays on the first project and nothing moves.

## English

**Set up the form**

1. Create a form in the Formgong dashboard and copy its access key.
2. In `index.html`, replace `fk_your_access_key` with that key.
3. The form sends `name`, `email`, `phone`, `service`, `message` and a hidden `subject`. Email and phone are required. It shows thanks only when Formgong answers `success: true`. If the answer is anything else, it shows the error and keeps what was typed.

**Edit**

- Colours are at the top of the styles: `--bg` for the dark page, `--accent` for the wordmark, buttons and arrows, `--light` for the service cards and the contact section.
- Each slide is an `<article class="slide">` with a photo, a title and a button. The script splits the title into letters and changes slides every 5000 ms (`DELAY` in the script).
- The numbers use `data-count` for the value they count up to.
- Replace the photos in `img/`, keeping the file names, or change the paths in `index.html`.

**Images.** The thirteen photos were generated for this template with ChatGPT image generation (OpenAI) and saved as WebP, about 1.2 MB in all. The buildings, rooms and the person are fictional. You may use them in your own site, but replace them with your own work before launch.

The "Powered by Formgong" links point to `https://formgong.com/review-page/fk_your_access_key`, so the same find and replace covers them. Once your key is in, the first click from your published site makes your own public review page on Formgong, where clients read and leave reviews, and every later click opens it. Switch the page off in Formgong (Reviews → your site → Settings) or change those links.

## Українська

Темний односторінковий сайт для студії дизайну інтер'єру чи архітектури. Студія Kavelle, засновниця, проєкти й цифри вигадані.

На сторінці:

- шапка з логотипом посередині, яка над слайдером прозора, а під час прокрутки стає темною;
- слайдер на п'ять проєктів на весь екран: фото змінюються кожні 5 секунд, назва з'являється літера за літерою;
- три категорії проєктів у ряд, який можна тягнути вбік;
- філософія студії з портретом засновниці;
- чотири картки послуг: клік вписує тему у форму;
- цифри студії, що рахуються;
- світлий блок контактів з бігучим заголовком і формою;
- футер.

**Налаштування.** Створіть форму в кабінеті Formgong і замініть `fk_your_access_key` у `index.html` на свій ключ. Подяка з'являється лише тоді, коли Formgong відповідає `success: true`.

**Зображення:** тринадцять фото згенеровано для цього шаблону в ChatGPT (OpenAI) і збережено у WebP, разом близько 1,2 МБ. Будівлі, кімнати й людина вигадані. Їх можна використовувати, але перед запуском замініть їх своїми роботами.

MIT license.

Посилання «Powered by Formgong» ведуть на `https://formgong.com/review-page/fk_your_access_key`, тож та сама заміна ключа оновить і їх. Коли ключ стоїть, перший перехід з вашого опублікованого сайту створює вашу публічну сторінку відгуків на Formgong, де клієнти читають і залишають відгуки; далі посилання відкриває її. Вимкнути сторінку можна у Formgong (Відгуки → ваш сайт → Налаштування) або змінити ці посилання.
