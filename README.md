# English Notebook

**Version 1.6.3**

English Notebook is a small app for learning words, phrases and grammar from your own lessons. It started as a way to practise the lessons from a YouTube English course, but it works for any language: you can learn English with Russian or Ukrainian translations, Spanish with English translations, and so on.

The app has no lessons built in. Each lesson is a small text file (a `.yaml` file) with the lesson's words, phrases and grammar. You add lesson files to the app, and it turns them into exercises and games.

It's free, needs no account and no installation, and works on phones and computers.

## Opening the app

There are two ways:

- **The link.** Open it in a browser (Chrome works best). This is the recommended way: app updates **and new lessons** arrive automatically. New lessons are published into the link's lessons folder, and the app picks them up the next time it's opened. If a lesson exists both there and as a hand-added file, the version from the link wins.
- **The file** `english-notebook.html`. Open it in any browser. It works without internet, but if the app gets updated, you need the new file.

## Lessons

Tap **Add a lesson** and pick one or more lesson files. They appear in the list, sorted by lesson number, and stay there: you only add a file once.

- Adding a file with the same lesson number again **updates** that lesson. Your progress is kept.
- A lesson can be **deleted** at the bottom of its page. If you add it again later, its progress comes back.
- Lessons are shown **10 per page**. The home screen always opens on the page with the lesson you're currently on.

## Inside a lesson

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

## How answers are checked

When you type an answer, the app is strict but fair:

- **Small typo** ("frend" for "friend") → *Almost!* You see the correct spelling.
- **Missing accent** ("adios" for "adiós", "mas" for "más") → counts as correct, with a reminder about the accents.
- **Missing article** ("house" for "a house") → counts as correct, with a reminder about the article.
- **Short forms** ("I'm" and "I am", "I'd like" and "I would like") → both are correct.
- **Another correct word** that isn't the one being learned ("do" instead of "make") → *That works too, but this lesson teaches: make.* It doesn't count as correct, but it isn't counted as a mistake either.
- If the app marks you wrong but you're sure you were right, tap **I was right**.

## Daily review

Everything you've answered goes into your daily review. Words come back after **1 day**, then **3, 7, 14, 30 and 60 days**, as long as you keep getting them right. A mistake moves a word **two steps back** (for example from the 30-day stage to the 7-day stage), and it comes back tomorrow. A word only loses steps once a day, however often it's missed that day.

The orange card on the home screen shows how many cards are waiting today (up to 20 per session). Once you're done, it turns green and shows how many are waiting tomorrow. Ten minutes of review a day is the best way to not forget old words while learning new ones.

## Vocabulary

The **book icon** at the top of the home screen (and on lesson pages and in Settings) opens the vocabulary: every word and phrase of the course with its translation and **0 to 5 stars**.

- A word gets 1 star after the first correct answer, then one more for each review it passes (after 1, 3, 7, 14 and 30 days). **5 stars means it's learned for the long run.**
- A mistake costs **2 stars** (never below 0), and the word comes back in tomorrow's review.
- Words marked *review today* are waiting in today's daily review; *not studied yet* means it hasn't come up yet.
- There's a **search** (in either language), a switch between words and phrases, sorting **by lesson**, **weakest first** or **A–Z**, and 20 entries per page.
- It isn't available during tests or exercises.

## Games and practice

- **Tricky words** – every word you've made mistakes with, until you get it right.
- **Pairs** – match 6 words with their translations as fast as you can. Your best time is saved.
- **Speed** – 45 seconds of "true or false?" with a word and a translation. Your best score is saved.

## Tests

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

## Progress

The home screen shows your **streak** (days in a row you practised), **words learned** (words you've typed correctly) and your **stars**.

Progress is saved **in your browser**, on your device. It stays after closing the browser or restarting the phone. It's lost only if you clear your browser data, use an incognito window, or switch to another browser or device.

In **Settings**:

- **Backup code** – copy a code that holds all your progress and lessons. Save it somewhere (notes, a message to yourself), and paste it back on any device to restore everything.
- **Reset all progress** – clears stars, records, streak and word stats. Your lessons stay. To reset just one lesson, use the link at the bottom of that lesson's page.

## Languages

- **Interface language:** English, Russian or Ukrainian, in Settings. On *Auto*, it follows the translation language of your lessons.
- **Courses:** each lesson file says which language is being learned and which language the translations are in. Every language being learned is its own course, with its own lessons and progress. If you have more than one, buttons at the top of the home screen switch between them. Lessons in one course can have translations in different languages; on *Auto*, the interface follows the newest lesson.

## Writing a lesson file

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

## Versions

The version number is at the bottom of the home screen and in Settings.

Version numbers follow three rules: the last number goes up for fixes, renames and small changes (1.4.1); the middle one for new features (1.5.0); the first one only if old lesson files or saved progress stop working (2.0.0).

| Version | What changed |
|---|---|
| 1.6.3 | Missing accents count as correct, with a reminder |
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

