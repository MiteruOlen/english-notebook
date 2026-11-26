# English Notebook

**Version 2.1.0**

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

**Sections.** A course can be split into sections: levels (A1, A2…) or topics (food, travel…). A lesson file says which one with `section: A2`, and lesson numbers start again at 1 in each section. When a course has more than one section, buttons under the course choose which one the lesson list shows (lessons without a section are under *Other*). Tests belong to a section too: `covers: [1, 2]` means lessons 1 and 2 of the test's own section. The daily review, games and vocabulary cover the whole course.

To move lessons you already have into a section, add `section:` to their files and add them again: each one replaces its copy without a section, and keeps its progress.

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

- **Small typo** ("frend" for "friend") → *Almost!* You see the correct spelling. It isn't counted as a mistake: the word comes back later in the same round, and getting it right then counts. (In a test a typo is still wrong for the score.)
- **Missing accent** ("adios" for "adiós", "mas" for "más") → counts as correct, with a reminder about the accents.
- **Missing article** ("house" for "a house") → counts as correct, with a reminder about the article.
- **Short forms** ("I'm" and "I am", "I'd like" and "I would like") → both are correct.
- **Another correct word** that isn't the one being learned ("do" instead of "make") → *That works too, but this lesson teaches: make.* It doesn't count as correct, but it isn't counted as a mistake either.
- If the app marks you wrong but you're sure you were right, tap **I was right**.

## Daily review

Every word and phrase you go through in a lesson joins your daily review, at **0 stars**, and comes up the next day. **Only the daily review moves a word on:** each time you get it right on its day it gains a star and comes back later: after **1 day**, then **3, 7, 14, 30 and 60 days**. A mistake in the review costs **two stars** (for example from the 30-day stage to the 7-day stage), and the word comes back tomorrow. A word gains or loses stars at most once a day.

Lessons, *Repeat lesson*, the games, *Tricky words*, *Practise these* and tests are practice: they never change a word's stars, its review date or its mistake count. A mistake in a lesson only lowers that step's stars. A second round of *Retry mistakes* after a review is practice too.

The orange card on the home screen shows how many cards are waiting today. A session has up to 20; when it ends, **Next 20** carries on with the rest (there's no point replaying the same 20: they're done for today). Once you're done, it turns green and shows how many are waiting tomorrow. Ten minutes of review a day is the best way to not forget old words while learning new ones.

## Vocabulary

The **book icon** at the top of the home screen (and on lesson pages and in Settings) opens the vocabulary: every word and phrase of the course with its translation and **0 to 5 stars**.

- A word starts at **0 stars** once you've gone through it in a lesson, then gets one more star for each daily review it passes on its day. **5 stars means it's learned for the long run.**
- A mistake in the daily review costs **2 stars** (never below 0), and the word comes back tomorrow. Mistakes anywhere else don't count here.
- Words marked *review today* are waiting in today's daily review; *not studied yet* (the **New** filter) means you haven't gone through it in a lesson yet.
- There's a **search** (in either language) and a switch between words and phrases.
- **Sort:** by lesson, weakest first, strongest first, next review, most mistakes, recently studied, A–Z or Z–A.
- **Show:** all, new, learning, learned, review today, or words with mistakes. Each button shows how many words it has; the three tiles at the top work as the same filters.
- **Lesson:** all lessons or just one. Search, lesson and *Show* work together (say, *lesson 8 · with mistakes*).
- **Per page:** 20, 50, 100 or all, with page buttons above and below the list. Each row shows its lesson, when it's due next and how many mistakes it has had.
- **Practise these** starts a round with up to 20 words from the list as it's filtered. It's practice only: stars don't change.
- **Hide a word** with the ⊘ button on its row, for words you don't want to learn yet. A hidden word is left out of lessons, the daily review, games, *Tricky words* and tests; its stars and review date wait for it. **Show → Hidden** lists them, and the same button brings a word back. In a lesson's word list, hidden words are struck through.
- With sections, the lesson filter is grouped by section, with *All of A1* and so on.
- Sort, *Show*, lesson and page size are remembered.
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

Progress is saved **in your browser**, on your device. Nothing is sent anywhere: the app has no accounts, no tracking, and it can't load anything from other websites (it only reads lesson files from its own lessons folder). It stays after closing the browser or restarting the phone. It's lost only if you clear your browser data, use an incognito window, or switch to another browser or device.

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
section: A1         # optional: a level or a topic
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
- `section` is optional. Lessons with the same section are numbered together (see *Sections* above).
- `words` and `phrases` are written as "word: translation". A hint can go in brackets at the end: `watch: дивитися (телевізор)`.
- `also` lists other correct words that aren't what the lesson teaches.
- In `grammar`, the **correct option goes first** inside the square brackets, and the whole line is wrapped in quotes.

Full rules and style conventions are written at the top of `lesson-01.yaml`. If a file has a mistake, the app says which file and which line.

## Keyboard

In lessons and tests the keyboard can do everything:

- **Tab** moves only between the answer box and the buttons of the exercise, in a loop (it never jumps to the browser). After you check a typed answer the cursor stays in the box: **Enter** goes on, **Tab** goes to *I was right*, then *Next*, then back to the box.
- **Multiple choice and grammar:** **1–4** pick an option.
- **Build the phrase:** every word shows its key. **1–9, 0, Q–P** pick a word, **Backspace** takes the last one back, **Enter** checks and then goes on.
- **Flashcards:** **Space** flips the card, then **1** = still learning, **2** = I know.

These are the defaults. **Settings → Keyboard** lets you choose, for each exercise:

| Exercise | Choices |
|---|---|
| Build the phrase | **1 2 3** (as above) · **Q W E**: letter keys only, no numbers · **Type**: type the first letters of a word, it's picked as soon as only one word fits · **Type + Space**: type a word (or its start) and press Space, like normal typing |
| Multiple choice and grammar | **1 2 3 4** · **A S D F** |
| Flashcards | **1 / 2** · **← / →** |

In the typing modes, **Backspace** removes a letter (or the last word), **Esc** clears what you typed, **-** picks a lone dash, and when one word is the start of another (*la / las*) **Space** picks the shorter one. You can also switch off the key hints once you know them.

The key labels and hints are hidden on phones and tablets.

## Versions

The version number is at the bottom of the home screen and in Settings.

Version numbers follow three rules: the last number goes up for fixes, renames and small changes (1.4.1); the middle one for new features (1.5.0); the first one only if old lesson files or saved progress stop working (2.0.0).

| Version | What changed |
|---|---|
| 2.1.0 | Hide words (and bring them back) from the vocabulary page; sections for levels or topics, with lesson numbers per section |
| 2.0.1 | Fix: "I was right" after a small typo in the review could set a word to an old star count |
| 2.0.0 | Only the daily review changes a word's stars and mistakes; lessons, games, practice and tests just add new words at 0 stars |
| 1.9.0 | Vocabulary: more sorts, filters by status and lesson, page size, page buttons on top, "Practise these" |
| 1.8.0 | Settings → Keyboard: choose the keys for each exercise, including typing words in Build the phrase; key hints can be switched off. Safer handling of pasted backup codes |
| 1.7.2 | A small typo is no longer a mistake: no penalty, the word comes back in the same round |
| 1.7.1 | Daily review: "Next 20" continues with the remaining words instead of replaying the same 20 |
| 1.7.0 | Keyboard: Tab stays inside the exercise, number keys for building phrases and flashcards |
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

