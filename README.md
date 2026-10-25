# English Notebook

**Version 1.6.2** · [English](#english) · [Українська](#українська)

---

## English

English Notebook is a small app for learning words, phrases and grammar from your own lessons. It started as a way to practise the lessons from a YouTube English course, but it works for any language: you can learn English with Russian or Ukrainian translations, Spanish with English translations, and so on.

The app has no lessons built in. Each lesson is a small text file (a `.yaml` file) with the lesson's words, phrases and grammar. You add lesson files to the app, and it turns them into exercises and games.

It's free, needs no account and no installation, and works on phones and computers.

### Opening the app

There are two ways:

- **The link.** Open it in a browser (Chrome works best). This is the recommended way: app updates **and new lessons** arrive automatically. New lessons are published into the link's lessons folder, and the app picks them up the next time it's opened. If a lesson exists both there and as a hand-added file, the version from the link wins.
- **The file** `english-notebook.html`. Open it in any browser. It works without internet, but if the app gets updated, you need the new file.

### Lessons

Tap **Add a lesson** and pick one or more lesson files. They appear in the list, sorted by lesson number, and stay there: you only add a file once.

- Adding a file with the same lesson number again **updates** that lesson. Your progress is kept.
- A lesson can be **deleted** at the bottom of its page. If you add it again later, its progress comes back.
- Lessons are shown **10 per page**. The home screen always opens on the page with the lesson you're currently on.

### Inside a lesson

Each lesson is a short path of steps. The next step is highlighted.

1. **Rule** – the grammar rule of the lesson, with an example.
2. **Flashcards** – flip each card and say whether you know the word.
3. **Words: choose** – pick the right translation from four options.
4. **Words: type** – see the translation, type the word yourself.
5. **Phrases: build** – put a sentence together from shuffled words.
6. **Phrases: type** – type the whole sentence.
7. **Grammar** – pick the right form: "She [watches / watch] TV."
8. **Game: pairs** – match words with their translations against the clock.

A lesson only has the steps it has material for: no phrases means no phrase steps.

**Stars.** Each step gives up to 3 stars, based on how many answers were right on the first try (3 stars for 95% or more, 2 for 80%, 1 for 50%). Your best result is saved, so you can always try again to improve it.

**Mistakes come back.** A wrong answer returns a few questions later in the same round, until you get it right. At the end you see a list of your mistakes and can practise just those.

**Repeat lesson** mixes words, phrases and grammar from the whole lesson into one quick review.

### How answers are checked

When you type an answer, the app is strict but fair:

- **Small typo** ("frend" for "friend") → *Almost!* You see the correct spelling.
- **Missing accent** ("adios" for "adiós") → *Almost! Check the accents.*
- **Missing article** ("house" for "a house") → counts as correct, with a reminder about the article.
- **Short forms** ("I'm" and "I am", "I'd like" and "I would like") → both are correct.
- **Another correct word** that isn't the one being learned ("do" instead of "make") → *That works too, but this lesson teaches: make.* It doesn't count as correct, but it isn't counted as a mistake either.
- If the app marks you wrong but you're sure you were right, tap **I was right**.

### Daily review

Everything you've answered goes into your daily review. Words come back after **1 day**, then **3, 7, 14, 30 and 60 days**, as long as you keep getting them right. A mistake moves a word **two steps back** (for example from the 30-day stage to the 7-day stage), and it comes back tomorrow. A word only loses steps once a day, however often it's missed that day.

The orange card on the home screen shows how many cards are waiting today (up to 20 per session). Once you're done, it turns green and shows how many are waiting tomorrow. Ten minutes of review a day is the best way to not forget old words while learning new ones.

### Vocabulary

The **book icon** at the top of the home screen (and on lesson pages and in Settings) opens the vocabulary: every word and phrase of the course with its translation and **0 to 5 stars**.

- A word gets 1 star after the first correct answer, then one more for each review it passes (after 1, 3, 7, 14 and 30 days). **5 stars means it's learned for the long run.**
- A mistake costs **2 stars** (never below 0), and the word comes back in tomorrow's review.
- Words marked *review today* are waiting in today's daily review; *not studied yet* means it hasn't come up yet.
- There's a **search** (in either language), a switch between words and phrases, sorting **by lesson**, **weakest first** or **A–Z**, and 20 entries per page.
- It isn't available during tests or exercises.

### Games and practice

- **Tricky words** – every word you've made mistakes with, until you get it right.
- **Pairs** – match 6 words with their translations as fast as you can. Your best time is saved.
- **Speed** – 45 seconds of "true or false?" with a word and a translation. Your best score is saved.

### Tests

A test is a separate file, like `test-05.yaml`. It has no words of its own: it asks questions from the lessons it covers (for example lessons 1–4), in a new mix every time.

- It appears in the list among the lessons, marked **Test**.
- To start it, you need the **teacher's code**. The teacher decides when the test happens.
- Each question is asked once, with no hints. The right answers are shown only at the end.
- There's a **time limit** (15 minutes by default). The timer doesn't pause, even if the page is reloaded. When time runs out, or the test is closed with the cross, it ends and gets graded.
- The result is a **grade from 1 to 5** (5 for 90% or more, 4 for 75%, 3 for 50%, 2 for 25%), the percent, and a list of mistakes with the right answers. It's saved with the date.
- A test is taken **once**. It can't be retaken, and resetting progress doesn't unlock it.
- **Copy the result for your teacher** copies the grade and the list of mistakes as text, ready to send in a message.
- The test file only holds a scrambled version of the code, so the code can't be read from it.

This is for discipline, not security: there's no server, so it can't stop someone determined to cheat.

### Progress

The home screen shows your **streak** (days in a row you practised), **words learned** (words you've typed correctly) and your **stars**.

Progress is saved **in your browser**, on your device. It stays after closing the browser or restarting the phone. It's lost only if you clear your browser data, use an incognito window, or switch to another browser or device.

In **Settings**:

- **Backup code** – copy a code that holds all your progress and lessons. Save it somewhere (notes, a message to yourself), and paste it back on any device to restore everything.
- **Reset all progress** – clears stars, records, streak and word stats. Your lessons stay. To reset just one lesson, use the link at the bottom of that lesson's page.

### Languages

- **Interface language:** English, Russian or Ukrainian, in Settings. On *Auto*, it follows the translation language of your lessons.
- **Courses:** each lesson file says which language is being learned and which language the translations are in. Every language being learned is its own course, with its own lessons and progress. If you have more than one, buttons at the top of the home screen switch between them. Lessons in one course can have translations in different languages; on *Auto*, the interface follows the newest lesson.

### Writing a lesson file

A lesson file is plain text. A small example:

```yaml
learn: en          # the language being learned
native: uk         # the language of the translations
lesson: 5
title: Present Simple
rule: |
  After **he / she / it** the verb gets **-s**: I work → he work**s**.
words:
  - work: працювати
  - a house: будинок
  - make: робити, створювати
    also: [do]
phrases:
  - I work here.: Я працюю тут.
grammar:
  - "She [works|work] here."
```

- `learn` and `native` are two-letter language codes. Without them, the app assumes English with Russian translations.
- `words` and `phrases` are written as "word: translation". A hint can go in brackets at the end: `watch: дивитися (телевізор)`.
- `also` lists other correct words that aren't what the lesson teaches.
- In `grammar`, the **correct option goes first** inside the square brackets, and the whole line is wrapped in quotes.

Full rules and style conventions are written at the top of `lesson-01.yaml`. If a file has a mistake, the app says which file and which line.

### Versions

The version number is at the bottom of the home screen and in Settings.

Version numbers follow three rules: the last number goes up for fixes, renames and small changes (1.4.1); the middle one for new features (1.5.0); the first one only if old lesson files or saved progress stop working (2.0.0).

| Version | What changed |
|---|---|
| 1.6.2 | Lessons published at the link win over hand-added copies |
| 1.6.1 | A mistake costs two review steps instead of resetting the word |
| 1.6.0 | Vocabulary page with stars for each word |
| 1.5.2 | "I'd" and "I would" count as the same |
| 1.5.1 | An extra article no longer counts as a mistake; saved test results are regraded |
| 1.5.0 | One course per language being learned, whatever the translation language |
| 1.4.1 | Tests are taken once, with no retakes; the result can be copied for the teacher |
| 1.4.0 | Tests: teacher's code, time limit, grade from 1 to 5 |
| 1.3.0 | "Days" renamed to "lessons" |
| 1.2.0 | Lessons shown 10 per page |
| 1.1.0 | "Also correct" answers, consistent articles in lesson files |
| 1.0.0 | First release: lessons from files, steps and stars, daily review, games, three interface languages |

---

## Українська

English Notebook — це невеликий застосунок для вивчення слів, фраз і граматики з ваших власних уроків. Він з'явився як спосіб практикувати уроки з курсу англійської на YouTube, але підходить для будь-якої мови: можна вчити англійську з російським чи українським перекладом, іспанську з англійським і так далі.

У застосунку немає вбудованих уроків. Кожен урок — це невеликий текстовий файл (файл `.yaml`) зі словами, фразами й граматикою уроку. Ви додаєте файли уроків у застосунок, а він перетворює їх на вправи та ігри.

Він безкоштовний, не потребує акаунта чи встановлення і працює на телефонах і комп'ютерах.

### Як відкрити застосунок

Є два способи:

- **Посилання.** Відкрийте його в браузері (найкраще в Chrome). Це рекомендований спосіб: оновлення застосунку **й нові уроки** приходять автоматично. Нові уроки публікуються в папку уроків при посиланні, і застосунок підхоплює їх, щойно його відкрити. Якщо урок є і там, і доданий вручну файлом, перемагає версія з посилання.
- **Файл** `english-notebook.html`. Відкрийте його в будь-якому браузері. Він працює без інтернету, але після оновлення застосунку потрібен новий файл.

### Уроки

Натисніть **Додати урок** і оберіть один або кілька файлів уроків. Вони з'являться у списку, упорядковані за номером уроку, і залишаться там: кожен файл додається лише один раз.

- Якщо знову додати файл з тим самим номером уроку, урок **оновиться**. Прогрес збережеться.
- Урок можна **видалити** внизу його сторінки. Якщо потім додати його знову, прогрес повернеться.
- Уроки показуються **по 10 на сторінці**. Головний екран завжди відкривається на сторінці з уроком, на якому ви зараз.

### Усередині уроку

Кожен урок — це короткий шлях із кроків. Наступний крок виділено.

1. **Правило** — граматичне правило уроку з прикладом.
2. **Картки** — переверніть кожну картку й скажіть, чи знаєте слово.
3. **Слова: вибір** — оберіть правильний переклад із чотирьох варіантів.
4. **Слова: написати** — бачите переклад, пишете слово самі.
5. **Фрази: скласти** — складіть речення з перемішаних слів.
6. **Фрази: написати** — напишіть усе речення.
7. **Граматика** — оберіть правильну форму: «She [watches / watch] TV.»
8. **Гра: пари** — з'єднайте слова з перекладами на швидкість.

В уроці є лише ті кроки, для яких є матеріал: немає фраз — немає кроків із фразами.

**Зірки.** Кожен крок дає до 3 зірок залежно від того, скільки відповідей були правильними з першої спроби (3 зірки — від 95%, 2 — від 80%, 1 — від 50%). Найкращий результат зберігається, тож завжди можна спробувати ще раз і покращити його.

**Помилки повертаються.** Неправильна відповідь повертається через кілька запитань у тому самому колі, доки ви не відповісте правильно. Наприкінці видно список помилок, і можна повторити лише їх.

**Повторити урок** змішує слова, фрази й граматику з усього уроку в одне швидке повторення.

### Як перевіряються відповіді

Коли ви пишете відповідь, застосунок суворий, але справедливий:

- **Невелика помилка в написанні** («frend» замість «friend») → *Майже!* Ви бачите правильне написання.
- **Пропущений знак над літерою** («adios» замість «adiós») → *Майже! Перевір знаки над літерами.*
- **Пропущений артикль** («house» замість «a house») → зараховується, з нагадуванням про артикль.
- **Скорочення** («I'm» і «I am», «I'd like» і «I would like») → обидва варіанти правильні.
- **Інше правильне слово**, але не те, що вивчається («do» замість «make») → *Так теж можна, але в цьому уроці вчимо: make.* Це не зараховується як правильна відповідь, але й помилкою не вважається.
- Якщо застосунок позначив відповідь як неправильну, а ви впевнені, що мали рацію, натисніть **Моя відповідь правильна**.

### Щоденне повторення

Усе, на що ви відповідали, потрапляє в щоденне повторення. Слова повертаються через **1 день**, потім через **3, 7, 14, 30 і 60 днів**, якщо ви й далі відповідаєте правильно. Помилка відкидає слово **на два щаблі назад** (наприклад, із 30-денного до 7-денного), і воно повертається завтра. За один день слово втрачає щаблі лише раз, хоч скільки разів у ньому помилилися.

Помаранчева картка на головному екрані показує, скільки карток чекає сьогодні (до 20 за раз). Коли все повторено, вона стає зеленою й показує, скільки карток чекає завтра. Десять хвилин повторення щодня — найкращий спосіб не забувати старі слова, поки вчиш нові.

### Словник

**Іконка книжки** вгорі головного екрана (а також на сторінках уроків і в Налаштуваннях) відкриває словник: усі слова й фрази курсу з перекладом і **від 0 до 5 зірок**.

- Слово отримує 1 зірку після першої правильної відповіді, а потім ще по одній за кожне пройдене повторення (через 1, 3, 7, 14 і 30 днів). **5 зірок — вивчено надовго.**
- Помилка забирає **2 зірки** (але не нижче 0), і слово повертається в завтрашнє повторення.
- Позначка *повторити сьогодні* — слово чекає в сьогоднішньому повторенні; *ще не вчили* — воно ще не траплялося.
- Є **пошук** (будь-якою з двох мов), перемикач між словами й фразами, сортування **за уроками**, **слабкі спочатку** або **А–Я** і по 20 записів на сторінці.
- Під час тестів і вправ словник недоступний.

### Ігри та практика

- **Складні слова** — усі слова, у яких були помилки, доки ви не відповісте правильно.
- **Пари** — з'єднайте 6 слів із перекладами якомога швидше. Найкращий час зберігається.
- **Швидкість** — 45 секунд «правильно чи ні?» зі словом і перекладом. Найкращий результат зберігається.

### Тести

Тест — це окремий файл, наприклад `test-05.yaml`. Власних слів у ньому немає: він ставить запитання з уроків, які охоплює (наприклад, з уроків 1–4), щоразу в новому наборі.

- Він з'являється у списку серед уроків із позначкою **Тест**.
- Щоб почати, потрібен **код від учителя**. Учитель вирішує, коли писати тест.
- Кожне запитання ставиться один раз, без підказок. Правильні відповіді показуються лише наприкінці.
- Є **обмеження часу** (типово 15 хвилин). Таймер не зупиняється, навіть якщо перезавантажити сторінку. Коли час виходить або тест закривають хрестиком, він закінчується й оцінюється.
- Результат — **оцінка від 1 до 5** (5 — від 90%, 4 — від 75%, 3 — від 50%, 2 — від 25%), відсоток і список помилок із правильними відповідями. Він зберігається разом із датою.
- Тест пишеться **один раз**. Перескласти його не можна, і скидання прогресу його не відкриває.
- **Скопіювати результат для вчителя** копіює оцінку та список помилок як текст, який можна надіслати в повідомленні.
- У файлі тесту зберігається лише зашифрований варіант коду, тож прочитати код із нього не можна.

Це для дисципліни, а не для безпеки: сервера немає, тож завадити тому, хто твердо вирішив схитрувати, застосунок не може.

### Прогрес

На головному екрані видно **серію** (скільки днів поспіль ви займалися), **вивчені слова** (слова, які ви правильно написали) і ваші **зірки**.

Прогрес зберігається **у вашому браузері**, на вашому пристрої. Він залишається після закриття браузера чи перезавантаження телефона. Він зникне, лише якщо очистити дані браузера, користуватися вікном інкогніто або перейти на інший браузер чи пристрій.

У **Налаштуваннях**:

- **Код прогресу** — скопіюйте код, у якому весь ваш прогрес і всі уроки. Збережіть його (у нотатках, у повідомленні собі) і вставте на будь-якому пристрої, щоб усе відновити.
- **Скинути весь прогрес** — очищає зірки, рекорди, серію й статистику слів. Уроки залишаються. Щоб скинути лише один урок, скористайтеся посиланням унизу сторінки цього уроку.

### Мови

- **Мова інтерфейсу:** англійська, російська або українська, у Налаштуваннях. У режимі *Авто* вона відповідає мові перекладів у ваших уроках.
- **Курси:** кожен файл уроку вказує, яку мову вивчають і якою мовою переклади. Кожна мова, яку вивчають, — окремий курс зі своїми уроками й прогресом. Якщо курсів кілька, кнопки вгорі головного екрана перемикають між ними. Уроки одного курсу можуть мати переклади різними мовами; у режимі *Авто* інтерфейс відповідає найновішому уроку.

### Як написати файл уроку

Файл уроку — це звичайний текст. Невеликий приклад:

```yaml
learn: en          # мова, яку вивчають
native: uk         # мова перекладів
lesson: 5
title: Present Simple
rule: |
  Після **he / she / it** до дієслова додаємо **-s**: I work → he work**s**.
words:
  - work: працювати
  - a house: будинок
  - make: робити, створювати
    also: [do]
phrases:
  - I work here.: Я працюю тут.
grammar:
  - "She [works|work] here."
```

- `learn` і `native` — двобуквені коди мов. Якщо їх немає, застосунок вважає, що це англійська з російським перекладом.
- `words` і `phrases` записуються як «слово: переклад». Підказку можна додати в дужках у кінці: `watch: дивитися (телевізор)`.
- `also` — інші правильні слова, які не є тим, що вивчається в уроці.
- У `grammar` **правильний варіант іде першим** у квадратних дужках, а весь рядок береться в лапки.

Повні правила й домовленості щодо стилю записані на початку файлу `lesson-01.yaml`. Якщо у файлі є помилка, застосунок покаже, у якому файлі та в якому рядку.

### Версії

Номер версії є внизу головного екрана й у Налаштуваннях.

Номери версій мають три правила: остання цифра зростає для виправлень, перейменувань і дрібних змін (1.4.1); середня — для нових можливостей (1.5.0); перша — лише якщо старі файли уроків або збережений прогрес перестають працювати (2.0.0).

| Версія | Що змінилося |
|---|---|
| 1.6.2 | Уроки, опубліковані при посиланні, мають перевагу над доданими вручну |
| 1.6.1 | Помилка забирає два щаблі повторення замість повного скидання |
| 1.6.0 | Сторінка словника з зірками для кожного слова |
| 1.5.2 | «I'd» і «I would» вважаються однаковими |
| 1.5.1 | Зайвий артикль більше не вважається помилкою; збережені результати тестів перераховуються |
| 1.5.0 | Один курс на кожну мову, яку вивчають, незалежно від мови перекладів |
| 1.4.1 | Тест пишеться один раз, без повторних спроб; результат можна скопіювати для вчителя |
| 1.4.0 | Тести: код від учителя, обмеження часу, оцінка від 1 до 5 |
| 1.3.0 | «Дні» перейменовано на «уроки» |
| 1.2.0 | Уроки показуються по 10 на сторінці |
| 1.1.0 | «Теж правильні» відповіді, єдині правила для артиклів у файлах уроків |
| 1.0.0 | Перший реліз: уроки з файлів, кроки й зірки, щоденне повторення, ігри, три мови інтерфейсу |
