<img src="logo.svg" width="96" alt="PariPariVault logo">

# PariPariVault

**A private archive of your TikTok likes and favorites, on your own computer.** For Windows 10/11.

*Formerly KaiVault. Updating from KaiVault keeps your archive, settings and TikTok login; the settings folder is renamed from KaiVault to PariPariVault on the first start.*

[По-русски ↓](#по-русски)

- **Everything stays with you.** Videos, captions and authors live in a folder on your disk. No servers,
  no accounts, no subscriptions. You can watch your archive offline.
- **Find any video in seconds.** Search by caption, author, hashtags and TikTok's own categories. Turn on speech
  search and it also finds what's said in the video and the text shown on screen.
- **Deleted on TikTok, still yours.** Creators delete videos and TikTok blocks them. PariPariVault marks the ones
  that are gone, and your copy stays.
- **Recognises videos you saved by hand.** Point it to a folder of old downloads. It works out which TikTok
  videos they are and adds author, caption, hashtags and categories. Your files are never moved or changed.

PariPariVault is not affiliated with TikTok or ByteDance. It only saves what *you* liked or added to favorites.

## Install

Download the [latest release](https://github.com/PariPariKai/PariPariVault/releases/latest):

- `PariPariVault-x.y.z-setup.exe` is the installer. It installs for your user only, so no admin rights are needed.
- `PariPariVault-x.y.z-portable.zip` runs without installing: unpack it anywhere and start `PariPariVault.exe`.
  Its settings stay next to it.

Requirements: Windows 10 or 11 (64-bit) and Microsoft Edge WebView2. WebView2 is already part of
Windows 11 and of almost every Windows 10. If yours lacks it, PariPariVault tells you where to get it.

> Windows SmartScreen may say "Windows protected your PC" because the app isn't code-signed.
> Click **More info → Run anyway**.

## Getting started

1. **Create an archive.** Pick a folder with plenty of space; a video takes about 5 MB on average.
2. **Request your data from TikTok.**
   - In the app: Profile → ☰ → Settings and privacy → Account → Download your data.
   - On the web: tiktok.com → Settings → Privacy → Download your data.
   - Choose the **JSON** format and select **Likes and favorites**. Also select **Your activity**,
     which holds your watch history; it helps recognise videos you saved by hand.
3. **Wait.** The file is ready after a few hours to a couple of days. Download the `.zip`; there's no need to unpack it.
4. **Drop the file into PariPariVault.** It shows how many videos it found; press the big button and it starts
   downloading, newest likes first, at a polite pace. Pause and resume whenever you like: it continues where it stopped.

The app walks you through these steps with a small animated guide, so you don't have to keep this page open.

PariPariVault reads **only the video lists** from the export. It never reads or sends anywhere your login history,
IP addresses, searches or messages.

TikTok puts only your **latest 6000 likes** in the export (favorites in full). Everything already in the archive
stays, so refresh the export every couple of months.

## Features

- Search by caption, author (`@name`), hashtag (`#tag`) and phrase (`"a few words"`). Partial words and
  case don't matter.
- Timeline by month, TikTok categories (Comedy › Pets › …), filters for dates, photos or videos, and likes or favorites.
- Player: ← → previous and next, ↑ ↓ volume, Esc to close. Clicking a transcript line jumps to that moment.
- 🎲 **Random** shows one random video, respecting the current filters. ✨ **Nostalgia** shows what you liked
  on these days in earlier years.
- The **Downloads** panel has one start/pause button, a live log, speed and time left, and shows why
  something wasn't saved:
  - deleted;
  - blocked in your country (a VPN may help);
  - 18+ (log in to TikTok in Settings).
- 🛡 **Check for deleted** goes through the archive and marks the videos TikTok no longer has.
- 📁 **My folders** recognises videos you saved by hand. This works best for videos saved with TikTok's
  own "Save video" button; forwarding through messengers strips the tags it relies on.
  If the folder you pick for the archive already has videos in it, PariPariVault offers to hook them up right away.
  Your own files are recognised first; only what is missing gets downloaded. The files are never moved or changed.
- **Speech search** is optional and downloaded on request:
  - with an NVIDIA graphics card: about 2.8 GB, and fast;
  - without one: about 0.5 GB on the CPU.
- yt-dlp, the download engine, updates itself weekly, because TikTok changes its site now and then.
- Russian and English interface.

## Where things are

| What | Where |
|---|---|
| Your archive (videos, database, exports) | the folder you chose. Back it up by copying this folder. |
| Settings, speech models, fresh yt-dlp | `%LOCALAPPDATA%\PariPariVault` (portable: `PariPariVault data` next to the exe) |

Uninstalling PariPariVault doesn't delete your archive or the downloaded models.

## Privacy

PariPariVault connects only to:
- TikTok, to download the videos you liked;
- Hugging Face and PyPI, to download speech models and yt-dlp updates, and only when you ask for them;
- GitHub, once a day, to see whether a new version of PariPariVault is out. The request carries nothing but the
  version you have.

**Updates.** When a new version is out, an **Update** button appears in the header. The installed version
downloads the new installer, checks it and installs it over the old one; the portable version sends you to the
release page for the new zip. Your archive and settings are never touched.

There is no telemetry. The local window talks to a local server on `127.0.0.1` that is protected
by a per-session key.

If you log in to TikTok for 18+ videos, you type your password on TikTok's own page. PariPariVault never sees it.
It stores the session cookies in your archive's `data` folder and uses them only for those videos.

## Support

PariPariVault is free and has no ads. If it's useful to you, you can say thanks:
[ko-fi.com/pariparikai](https://ko-fi.com/pariparikai). Feedback and ideas: [X — @Pariparikai](https://x.com/Pariparikai).

## License

© 2026 PariPariKai. All rights reserved. PariPariVault is free to use; the terms are in [`LICENSE`](LICENSE).
Bundled third-party components and their licenses are listed in [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md).

---

## По-русски

*Раньше программа называлась KaiVault. Обновление с KaiVault сохраняет архив, настройки и вход в TikTok; папка настроек при первом запуске переименовывается из KaiVault в PariPariVault.*

**PariPariVault — личный архив твоих лайков и избранного из TikTok на твоём компьютере.** Для Windows 10/11.

- **Всё хранится у тебя.** Видео, описания и авторы лежат в папке на диске. Никаких серверов, аккаунтов и подписок.
  Смотреть можно без интернета.
- **Любое видео находится за секунды.** Ищет по описанию, автору, хэштегам и категориям TikTok. Если включить
  поиск по речи — то и по тому, что говорят в видео, и по тексту на экране.
- **Удалят из TikTok — у тебя останется.** PariPariVault отмечает видео, которых в TikTok больше нет.
- **Узнаёт видео, сохранённые вручную.** Укажи папку со старыми загрузками — программа поймёт, что это за ролики,
  и подтянет автора, описание, хэштеги и категории. Сами файлы не двигаются и не меняются.

PariPariVault не связан с TikTok и ByteDance.

### Установка

Скачать: [последний релиз](https://github.com/PariPariKai/PariPariVault/releases/latest).

- `PariPariVault-x.y.z-setup.exe` — установщик. Права администратора не нужны.
- `PariPariVault-x.y.z-portable.zip` — версия без установки: распаковать куда угодно и запустить `PariPariVault.exe`.

Если Windows пишет «Система Windows защитила ваш компьютер», нажми **Подробнее → Выполнить в любом случае**.
Так бывает со всеми программами без платной цифровой подписи.

### Как начать

1. **Создай архив.** Выбери папку, где много места: в среднем около 5 МБ на видео.
   Если в папке уже лежат видео, скачанные из TikTok раньше, программа предложит их подключить:
   сначала узнает свои файлы и только потом докачает то, чего не хватает. Сами файлы не двигаются и не меняются.
2. **Закажи данные в TikTok.**
   - В приложении: Профиль → ☰ → Настройки и конфиденциальность → Аккаунт → Скачать данные.
   - На сайте: tiktok.com → Настройки → Конфиденциальность → Скачать данные.
   - Формат **JSON**. Отметь пункт **«Лайки и избранное»** и ещё **«Ваша активность»**: в ней история
     просмотров, она помогает узнать вручную скачанные видео.
3. **Подожди.** Файл готовится от пары часов до пары дней. Скачай `.zip`, распаковывать его не нужно.
4. **Перетащи файл в окно PariPariVault.** Программа покажет, сколько видео нашла; жми большую кнопку — и загрузка
   пойдёт, сначала свежие лайки. Ставь на паузу и продолжай когда угодно: она продолжит с того же места.

Все эти шаги программа показывает сама — маленьким анимированным гидом «куда тыкать».

Из экспорта читаются **только списки видео**. История входов, IP-адреса, поиски и сообщения не читаются и никуда
не отправляются. TikTok кладёт в файл только **последние 6000 лайков** (избранное — целиком). Всё, что уже есть
в архиве, останется, поэтому просто обновляй экспорт раз в пару месяцев.

### Где что лежит

- **Архив** (видео, база, экспорты) — в папке, которую ты выбрал. Для бэкапа просто скопируй её.
- **Настройки, модели распознавания, свежий yt-dlp** — `%LOCALAPPDATA%\PariPariVault`.
  В portable-версии — папка `PariPariVault data` рядом с программой.
- При удалении программы архив и модели остаются.

### Приватность

PariPariVault обращается только:
- к TikTok — чтобы скачать то, что ты лайкнул;
- к Hugging Face и PyPI — чтобы скачать модели распознавания и обновления yt-dlp, только когда ты сам это включишь;
- к GitHub — раз в сутки узнать, не вышла ли новая версия. В запросе только номер твоей версии.

**Обновления.** Когда выходит новая версия, в шапке появляется кнопка **«Обновление»**. Установленная версия сама
качает новый установщик, проверяет его и ставит поверх старой; portable-версия открывает страницу релиза с новым
zip. Архив и настройки не трогаются.

Телеметрии нет. Если войти в TikTok для видео 18+, пароль вводится на странице самого TikTok, и программа его
не видит.

### Поддержать

PariPariVault бесплатный и без рекламы. Если он тебе пригодился, можно сказать спасибо:
[dalink.to/pariparikai](https://dalink.to/pariparikai). Фидбек и идеи: [X — @Pariparikai](https://x.com/Pariparikai).
Автор ещё и стример: [Twitch — PariPariKai](https://www.twitch.tv/pariparikai).

### Лицензия

© 2026 PariPariKai. Все права защищены. Пользоваться программой можно бесплатно; условия — в [`LICENSE`](LICENSE).
Сторонние компоненты и их лицензии перечислены в [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md).
