---
last_updated: 2026-11-25
version: 6.0.1
link_for_spec: dev-docs/specs/USER_MANUAL_SPEC.instructions.md
product_versions:
  windows: "0.1.0"
  ios: "1.0.0"
  android: "1.0.0"
generated_from: "dev-docs/specs/USER_MANUAL_SPEC.instructions.md"
---

# User Manual

## Overview

Plain Vim Practice is a study aid for people learning the Vim text editor, such
as students, developers, and system administrators. It teaches 67 everyday Vim
commands in nine categories, explains them in six short guides, and checks what
you remember with quizzes, key-combo exercises, and 14 editing challenges in a
built-in Vim-style emulator.

| Item | Details |
| --- | --- |
| Platforms | iOS on iPhone and iPad on the App Store; Android phones and tablets on Google Play |
| Interface | Four tabs: **Home**, **Practice**, **Emulator**, and **Docs** |
| Version | 1.0.0 on iOS and Android |

<!-- Verified from: platform/ios/plain-vim-practice.xcodeproj/project.pbxproj [MARKETING_VERSION, TARGETED_DEVICE_FAMILY] -->
<!-- Verified from: platform/android/app/build.gradle.kts [versionName] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings.xml [tab_home, tab_practice, tab_emulator, tab_docs] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/CommandLibrary.kt [CommandLibrary.all] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Command.kt [CommandCategory] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/GuideLibrary.kt [GuideLibrary] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Challenge.kt [ChallengeLibrary] -->
<!-- Verified from: dev-docs/store_listings/app_store.md [App Review Notes] -->

The commands, guides, quizzes, key combos, emulator, and the first three
challenges are in the base plan. **Full Access**, an optional one-time purchase,
opens all 14 challenges. See [Unlock Full Access](#unlock-full-access).

Plain Vim Practice needs no account, shows no ads, and has no analytics or
tracking. It checks your answers on the device and works offline. Its only
network use is the store (the App Store on iOS, Google Play on Android), for
the price of Full Access and your purchases.

<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_services_body, docs_privacy_device_body] -->
<!-- Verified from: platform/ios/plain-vim-practice/PrivacyPolicyView.swift -->

Vim is free software by Bram Moolenaar and the Vim contributors. Plain Vim
Practice is an independent study aid by Plain Text Office LLC and is not
affiliated with or endorsed by the Vim project. Its emulator was written for
this app and contains no Vim code.

<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_about] -->

## Installation and Setup

### Check the System Requirements

| Requirement | Details |
| --- | --- |
| Device | iPhone or iPad, or an Android phone or tablet |
| Operating system | iOS 26 or later, or Android 8.0 or later |
| Account or sign-in | None required |
| Internet connection | Not required, except to buy or restore Full Access |
| Permissions | None requested |

<!-- Verified from: platform/ios/plain-vim-practice.xcodeproj/project.pbxproj [IPHONEOS_DEPLOYMENT_TARGET = 26.0] -->
<!-- Verified from: platform/android/app/build.gradle.kts [minSdk = 26] -->
<!-- Verified from: platform/android/app/src/main/AndroidManifest.xml [no permissions declared] -->

### Get the App

On an iPhone or iPad, install Plain Vim Practice from the
[App Store](https://apps.apple.com/app/plain-vim-practice/id6838480775).
On an Android phone or tablet, install it from
[Google Play](https://play.google.com/store/apps/details?id=com.plaintxtoffice.plainvimpractice).

<!-- Verified from: dev-docs/store_listings/app_store.md [Store Details] -->
<!-- Verified from: platform/android/app/build.gradle.kts [applicationId, versionName] -->

### Set Up the App

No setup is needed. The commands, guides, practice texts, and challenges are
included with the app, and your progress starts empty the first time you open
it.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/CommandLibrary.kt [CommandLibrary] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/data/AppDatabase.kt -->

## Starting the Program

### Open Plain Vim Practice

1. On your Home screen or in your app list, tap **Plain Vim Practice**.
1. The app opens on the **Home** tab, which shows a card for each of the other
   three tabs and a **Send Feedback** button.

<!-- Verified from: platform/android/app/src/main/res/values/strings.xml [app_name] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/home/HomeScreen.kt [HomeScreen, HomeDestination] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/HomeView.swift -->

### Close Plain Vim Practice

The app has no quit command. Leave it the way you leave any app on your device.
Learned marks, quiz answers, and challenge best scores are saved as you go. The
emulator's practice text is not saved: it is cleared when the app closes.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/EmulatorViewModel.kt [EmulatorViewModel] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/QuizViewModel.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengeViewModel.kt [recordSolve] -->

## Getting Around

The app has four tabs.

| Tab | What you find there |
| --- | --- |
| **Home** | A card for **Practice**, **Emulator**, and **Docs**, and **Send Feedback** |
| **Practice** | Quizzes and key-combo exercises |
| **Emulator** | The Vim-style editor with practice texts, and **Challenges** |
| **Docs** | **Commands** and **Guides**, switched with the control at the top; **About** is at the end of **Guides** |

<!-- Verified from: platform/android/app/src/main/res/values/strings_home.xml -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsScreen.kt [DocsScreen, AboutSection] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/DocsView.swift -->

- Tap a card on **Home** to switch to that tab.
- Each tab keeps its own screens. When you switch tabs and come back, you
  return to where you were.
- A quiz, a key-combo round, the challenges, and **Full Access** fill the
  screen without the tab bar. Close them with **Close**, **Done**, or
  **End Practice**.
- On Android, the tabs float in a bar at the bottom of the screen. On a wide
  screen, such as a tablet, they appear as a rail along the side instead.
  Tapping the tab you are already on returns it to its first screen.
- On Android, the system Back gesture or button closes the screen you are on.
  On the first screen of a tab other than **Home**, it returns to **Home**; on
  **Home**, it leaves the app.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/Navigation.kt [AppNavigation] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/NavigationKeys.kt [FullScreenKey] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/root/RootScreen.kt [RootLayout, RailMinWidth] -->

Help for Vim itself is in the **Docs** tab. Typing `:help` in the emulator
reminds you of that.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt ["Help is in the Docs tab"] -->

## Everyday Tasks

### Look Up a Command

1. Open the **Docs** tab and choose **Commands** at the top.
1. Browse the commands, grouped by category, or type in the search field
   (**Keys or task**).
1. Tap a command to open its page.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsScreen.kt [CommandSections, SearchField] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_search_hint] -->

The search matches a command's keys and its equivalent keys exactly as you type
them, because Vim's keys are case sensitive: `d` finds `dd` and `dw` but not
`D`. It matches words in a command's summary in any case, so `delete` finds the
delete commands. If nothing matches, the tab shows **No Results**.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsViewModel.kt [matchesSearch] -->

The nine categories are:

| Category | What it covers |
| --- | --- |
| Modes & Inserting | Switch between Normal and Insert mode. |
| Moving Around | Move the cursor by character, word, line, and file. |
| Deleting & Changing | Delete, change, replace, and join text. |
| Copy & Paste | Yank text and put it somewhere else. |
| Text Objects | Act on a whole word, quote, or bracket pair. |
| Search & Replace | Find text and replace it. |
| Visual Mode | Select text, then act on it. |
| Undo & Repeat | Undo, redo, and repeat changes. |
| Saving & Quitting | Write the file and leave Vim. |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Command.kt [CommandCategory] -->

A command page shows:

- The command's summary.
- **Syntax**, such as `[count]dd` or `f{char}`.
- **Same As**, other keys that do the same thing, when there are any.
- **Examples**, each with the keys to type and an explanation. Most show the
  text **Before** and **After** the keys, with the cursor position marked.
- A tip, for many commands.
- Your quiz record for the command, such as **Quiz record: 3 of 4 correct**,
  once you have answered a question about it.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/CommandDetailScreen.kt [CommandDetailScreen] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_syntax, docs_same_as, docs_examples, docs_quiz_record] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/CommandDetailView.swift -->

### Copy an Example

1. Open a command page or a guide.
1. Tap **Copy** next to a syntax line or an example.

The text goes on your device's clipboard, ready to paste into another app. Apps
you paste into, and apps allowed to read the clipboard, can read it.

<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_copy_body] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings.xml [copy, copied] -->

### Mark a Command as Learned

1. Open the command's page.
1. Tap **Mark as Learned** at the bottom of the page.

The button changes to **Learned**, and the command shows a check mark in the
**Commands** list. Tap **Learned** to remove the mark. A quiz on **Not Yet
Learned** leaves out the commands you have marked.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/CommandDetailScreen.kt [LearnedButton] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsScreen.kt [CommandRow] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeSettings.kt [practicePool] -->

### Read a Guide

1. Open the **Docs** tab and choose **Guides** at the top.
1. Tap a guide.

Each guide has a summary, then sections with worked examples. The six guides
are **Modes**, **Operators and Motions**, **Counts and Repeating**, **Text
Objects**, **Search and Replace**, and **Saving and Quitting**.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/GuideLibrary.kt [GuideLibrary] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/GuideScreen.kt -->

### Take a Quiz

1. Open the **Practice** tab.
1. Under **Quiz Type**, choose **Multiple Choice** (pick the right command from
   four choices) or **Type the Command** (read the description and type the
   keys).
1. Under **Commands**, open the menu and choose which commands to be quizzed
   on. Each choice shows how many commands it holds.
1. Set **Questions** with the minus and plus buttons, from 5 to 30 in steps of
   5. It starts at 10.
1. Tap **Start Quiz**.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeScreen.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Quiz.kt [QuizMode] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeSettings.kt [MIN_QUIZ_QUESTIONS, MAX_QUIZ_QUESTIONS, QUIZ_QUESTION_STEP, DEFAULT_QUIZ_QUESTIONS] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/PracticeView.swift [QuestionStepper] -->

| Choice | Commands it quizzes |
| --- | --- |
| **All Commands** | Every command |
| **Not Yet Learned** | Commands you have not marked as learned |
| **Needs Review** | Commands you keep missing: you have missed one at least once and answered fewer than 70% of its questions correctly |
| A category, such as **Text Objects** | The commands in that category |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeSettings.kt [GeneralScopes, CategoryScopes, practicePool] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/data/CommandProgress.kt [NEEDS_REVIEW_BELOW] -->

Each question is about a different command, so a quiz on a small category has
fewer questions than you chose. If **Needs Review** is empty, the tab says
**Nothing to review yet**.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Quiz.kt [QuizBuilder.makeQuestions] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_practice.xml [practice_nothing_to_review] -->

During the quiz:

1. Read the question. Most show what a command does; in **Multiple Choice**,
   some ask **Which command does the same as** another set of keys.
1. Tap a choice, or type the keys in the **Keys** field and tap **Check**.
1. The app shows **Correct!** or **Not quite. The answer is** with the right
   command.
1. Tap **Next Question**, or **See Results** after the last question.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/QuizScreen.kt -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_practice.xml [practice_quiz_alias_prompt, practice_quiz_keys_hint, practice_quiz_check, practice_quiz_correct, practice_quiz_incorrect, practice_quiz_next, practice_quiz_see_results] -->

Typed answers are case sensitive, as in Vim, and spaces around them are
ignored. An equivalent set of keys also counts, except in a question that
already shows it.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Command.kt [Command.matches] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Quiz.kt [QuizQuestion.isCorrect] -->

**Results** shows your score and lists the commands you missed under **Review
These**; tap one to open its page. Tap **Done** to finish. Every answer is
saved as you give it, so closing a quiz early with **Close** keeps the answers
you already gave.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/QuizScreen.kt [QuizRoute] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/QuizViewModel.kt -->

### Practice Key Combos

Key combos put several keys together to do one editing task, such as `daw` to
delete a word and the space after it.

1. Open the **Practice** tab.
1. Under **Key Combos**, choose **Pick the Keys** or **Build the Keys**.
1. Set **Questions**, from 1 to 20. It starts at 10, and the app remembers the
   number you choose for next time.
1. Tap **Start Combo Quiz**.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeScreen.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Combo.kt [ComboLibrary.all, ComboSession.DEFAULT_QUESTION_COUNT] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeSettings.kt [ComboQuestionCountSetting] -->
<!-- Verified from: platform/ios/plain-vim-practice/Models/Combo.swift [defaultQuestionCount] -->

Each question shows an editing task and the text it starts from.

- **Pick the Keys** (**Which keys do this?**): tap the choice that does the
  task, then tap **Check Answer**.
- **Build the Keys** (**Build the keys that do this.**): tap the pieces under
  **Pieces** in order. They appear under **Your Keys**; tap a placed piece to
  take it back out. One piece is a decoy that the answer does not need. Tap
  **Check Answer** when you are done.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/ComboScreen.kt -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_practice.xml [practice_combo_heading_pick, practice_combo_heading_build, practice_combo_check, practice_combo_your_keys, practice_combo_pieces, practice_combo_decoy] -->

**Combo Results** shows your score and lists the combos to review. To stop
early, tap **End Practice** and confirm. Combo answers are not saved; only
quiz answers count toward a command's record.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/ComboViewModel.kt -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_practice.xml [practice_combo_results_title, practice_combo_review, practice_combo_end, practice_combo_end_title] -->

### Try Commands in the Emulator

The **Emulator** tab is a small Vim-style editor for trying commands on a
practice text. It starts in Normal mode, as Vim does, so keys are commands
until you enter Insert mode.

1. Open the **Emulator** tab. The keyboard opens, and the practice text's file
   name, such as `welcome.txt`, is at the top.
1. Type Vim keys. The text changes as Vim would change it.
1. Watch the status line under the text. It shows the mode
   (`-- INSERT --`, `-- VISUAL --`, or `-- VISUAL LINE --`), the keys of a
   command you have not finished (**Typed so far**), messages such as
   `3 fewer lines` or an error, and the cursor's line and column.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/EmulatorScreen.kt [EmulatorRoute, EmulatorScreen] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/VimText.kt [VimStatusLine] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_mode_insert, emulator_mode_visual, emulator_mode_visual_line, emulator_typed_so_far] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/EmulatorView.swift -->

A row of keys above the keyboard holds keys the on-screen keyboard lacks or
hides:

| Key | What it does |
| --- | --- |
| **Esc** | Leaves Insert or Visual mode, or cancels a half-typed command |
| **Ctrl-R** | Redo |
| `:` `/` `.` `$` `^` `0` `%` `"` `(` `)` `{` `}` `*` | Types that character |
| Keyboard button (last in the row) | Hides the on-screen keyboard, or shows it again |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/VimText.kt [VimKeyRow, KeyRowSymbols, KeyboardToggle] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/EmulatorView.swift [EmulatorKeyRow] -->

The row scrolls sideways when it does not fit. Tap the text to bring the
keyboard back after hiding it. A hardware keyboard works too; see
[Use a Hardware Keyboard](#use-a-hardware-keyboard).

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/VimText.kt [VimBuffer onShowKeyboard] -->

The emulator covers the commands the app teaches: Normal, Insert, Visual, and
command-line modes; counts, motions, operators, and text objects; search;
undo, redo, and `.`; and a handful of `:` commands. It differs from Vim on
purpose in a few ways: search and `:s` patterns are plain text, not regular
expressions; indenting uses four spaces; and there is one register for yanked
and deleted text. Keys it does not know are ignored or answered with Vim's own
error message.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt [VimEngine] -->

The emulator never opens or saves files on your device. `:w` reports writing
the practice text, and `:q` and `:wq` show that Vim would close here, but the
emulator stays open. Your edits last while the app runs and are cleared when it
closes.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt [writeBuffer, requestExit] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_device_body] -->

### Choose a Practice Text

1. In the **Emulator** tab, tap the **Practice Text** button at the top
   right.
1. Choose a text. It replaces the one you were editing.

| Practice text | File name | What it holds |
| --- | --- | --- |
| **Welcome** | `welcome.txt` | A short introduction to the emulator's keys, with a deliberate typo to fix |
| **Code** | `greet.py` | A short Python program |
| **List** | `list.txt` | A shopping and errands list, with a repeated line |
| **Empty** | `new.txt` | An empty text |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/PracticeText.kt [PracticeText] -->

To undo all your edits, choose **Start Over** in the same menu, or type `:q!`
and press Return.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/EmulatorScreen.kt [PracticeTextMenu] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt ["q", "quit"] -->

### Solve a Challenge

A challenge asks you to turn one text into another in as few keys as you can.
Par is the number of keys in the app's own answer.

1. In the **Emulator** tab, tap **Challenges** at the top left.
1. Tap a challenge. Each row shows its par and, once solved, your best count.
1. Read the goal and the **Target** text, then edit the text with Vim keys.
   The count of keys you have pressed is shown as **Keys** beside **Par**.
1. When the text matches the target and you are back in Normal mode, the
   challenge is solved. Press **Esc** after typing in Insert mode; it counts
   as a key.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengesScreen.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengeScreen.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Challenge.kt [ChallengeRun.isSolved, ChallengeRun.press] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_challenge_target, emulator_challenge_keys, emulator_challenges_footer_unlocked] -->

The result shows how many keys you used and how that compares with par, such
as **On par.** or **2 under par. Better than our answer!** Tap **Try Again** to
start over, or **Next Challenge** to go on. Your best count for each challenge
is saved, and a challenge solved at par or better is marked as such in the
list.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_challenge_on_par, emulator_challenge_under_par, emulator_challenge_over_par, emulator_challenge_next, emulator_challenge_solved_at_par] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengeViewModel.kt [recordSolve] -->

While you work, the **Challenge Options** menu offers **Start Again**, to reset
the text and the key count, and **Show Our Answer**, which shows the app's
keys for the challenge. Tap **Done** in the list to return to the emulator. On
iOS, the challenges open as a sheet over the **Emulator** tab; on Android, they
fill the screen.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengeScreen.kt [ChallengeOptions] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/EmulatorView.swift [sheet] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/NavigationKeys.kt [ChallengesKey] -->

The 14 challenges, in order, are Fix the Typo, One Line Too Many, A Change of
Drink, Out of Order, Inside the Quotes, No Arguments, All on One Line, Three
Words Fewer, Indent the Block, Four of a Kind, Trim the Line, Say It Loud,
Repeat Yourself, and Cats to Dogs. The first three are in the base plan; the
rest show **Needs Full Access** until you unlock them.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Challenge.kt [ChallengeLibrary.entries, FREE_COUNT] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_challenge_locked] -->

### Unlock Full Access

**Full Access** is a paid, optional one-time purchase that opens challenges
4 to 14. Without it, you have the commands, guides, quizzes, key combos, the
emulator, and the first three challenges. It is not a subscription, and it works
offline once bought. It is sold through the App Store on iOS and through Google
Play on Android (in development). The store shows the price.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_intro, emulator_unlock_feature_footer, emulator_unlock_footer] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/premium/Entitlement.kt [FULL_ACCESS_PRODUCT_ID] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/UnlockView.swift -->

1. Open the **Full Access** screen in one of these ways:
   - In the **Emulator** tab, tap **Challenges**, then a locked challenge.
   - Tap **Next Challenge** after solving the last challenge you can open.
   - In the **Docs** tab, choose **Guides**, then tap **Full Access** under
     **About**. The row shows **Unlocked** or **Not unlocked**.
1. Tap **Unlock for** and the price.
1. Complete the purchase in the store's payment sheet.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengesScreen.kt [onOpenUnlock] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/ChallengeScreen.kt [onOpenUnlock] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsScreen.kt [FullAccessRow] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_buy] -->

The screen then shows **Full access unlocked. Thank you!** and **Full Access is
unlocked.** If the purchase needs approval, such as from a family manager, it
shows **Your purchase is waiting for approval** and Full Access starts once it
is approved.

<!-- Verified from: platform/android/app/src/main/res/values/strings.xml [full_access_notice_purchased, full_access_notice_pending] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_unlocked] -->

Full Access stays with the account you bought it with: your Apple Account on
iOS, or your Google Account on Android.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_footer] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/UnlockView.swift -->

On Android, **Have an access code?** on the Full Access screen unlocks Full
Access on this device for someone who was given a code, such as an app
reviewer. It is not needed to buy Full Access.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_code_prompt, emulator_unlock_code_footer] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/premium/FullAccess.kt [redeemAccessCode] -->

### Restore Full Access

Use this on a new device, or after reinstalling the app, signed in to the same
account you bought Full Access with.

1. Open the **Full Access** screen.
1. Tap **Restore Purchases**.

The screen shows **Full access restored.** or that no Full Access purchase was
found for the account. On Android, the app also checks Google Play for your
purchase each time it starts and each time you return to it.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_restore] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings.xml [full_access_notice_restored, full_access_notice_not_found] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/premium/FullAccess.kt [start, foregroundEvents] -->

### Reset All Progress

This clears learned marks, quiz history, and challenge best scores. It cannot
be undone.

1. Open the **Docs** tab and choose **Guides**.
1. Under **About**, tap **Reset All Progress**. It is dimmed while there is
   nothing to clear.
1. In **Reset all progress?**, tap **Reset**, or **Cancel** to keep your
   progress.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsScreen.kt [ResetRow, ResetDialog] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_reset_all_progress, docs_reset_title, docs_reset_message, docs_reset_confirm] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/DocsView.swift -->

Reset does not remove Full Access, which belongs to your store account.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/DocsViewModel.kt [resetProgress] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/premium/FullAccess.kt [FullAccess] -->

### Read the Privacy Policy

Open the **Docs** tab, choose **Guides**, and tap **Privacy** under **About**.
**Contact Plain Text Office**, at the end, opens the contact page in your
browser. On Android, the policy also has a **Google Play diagnostics** section.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/PrivacyScreen.kt -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_diagnostics_title, docs_privacy_contact] -->
<!-- Verified from: platform/ios/plain-vim-practice/PrivacyPolicyView.swift -->

## Settings and Preferences

The app has no settings screen. It remembers one choice between launches.

| Setting | Default | Accepted values | How to change it |
| --- | --- | --- | --- |
| Key-combo **Questions** | 10 | 1 to 20 | Use the minus and plus buttons under **Key Combos** in the **Practice** tab |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeSettings.kt [ComboQuestionCountSetting, SharedPreferencesPracticeSettingsStore] -->
<!-- Verified from: platform/ios/plain-vim-practice/Models/Combo.swift [questionCount] -->

The quiz type, the commands to quiz on, and the quiz length go back to their
starting values (**Multiple Choice**, **All Commands**, and 10 questions) the
next time you open the app. In the emulator, `:set nonumber` hides the line
numbers and `:set number` shows them again, until the app closes.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeViewModel.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt ["set", "se"] -->

## Importing and Exporting

Not Applicable.
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice (no import or export features; the emulator opens and saves no files) -->

## Commands and Shortcuts

### Use a Hardware Keyboard

In the emulator and the challenges, a hardware keyboard types Vim keys
directly. These key presses have their Vim meaning:

| Key | What it does |
| --- | --- |
| **Esc** | Escape |
| **Ctrl+[** | Escape |
| **Ctrl+R** | Redo |
| **Backspace** | Backspace |
| **Return** or **Enter** | Enter |

On Android, other **Ctrl** combinations are left to the system. With a
hardware keyboard you can hide the on-screen keyboard with the last button in
the key row, and keys still reach the emulator.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/emulator/VimKeyInput.kt [hardwareVimKey, VimKeyboard.hide] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/VimKeyInput.swift [keyCommands] -->

### Emulator Commands

These `:` commands work in the emulator. Type them in Normal mode and press
Return.

| Command | What it does |
| --- | --- |
| `:w` | Reports writing the practice text; nothing is saved to your device |
| `:q` | Shows that Vim would close; refuses with error E37 if there are unsaved changes |
| `:q!` | Undoes all changes since the last `:w` |
| `:wq` or `:x` | Reports writing, then shows that Vim would close |
| `:s/old/new/` or `:%s/old/new/g` | Replaces plain text on the current line or a range, with the `g` flag for every match |
| `:d` | Deletes the current line or a range of lines |
| `:u` and `:redo` | Undo and redo |
| `:{number}` | Moves to that line |
| `:set number` and `:set nonumber` | Shows or hides line numbers |
| `:noh` | Accepted; the emulator does not highlight matches |
| `:help` | Points you to the **Docs** tab |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt [command-line commands, substitute, writeBuffer, requestExit] -->

For Normal-mode keys, see the **Commands** list in the **Docs** tab.

## Your Data Files

Plain Vim Practice keeps your progress inside the app on your device. You
cannot open or edit these files by hand, and nothing is sent to Plain Text
Office.

| What is kept | Where |
| --- | --- |
| Learned marks, quiz answer counts, the date you last practiced each command, and challenge best scores | The app's own storage |
| The key-combo question count you chose | The app's own storage |
| The emulator's practice text | Memory only; cleared when the app closes |

<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_device_body] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/data/AppDatabase.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/practice/PracticeSettings.kt [SharedPreferencesPracticeSettingsStore] -->

On Android, the progress is in a database and the key-combo count in a
preferences file, both in the app's private storage, which other apps cannot
read. Clearing the app's storage in Android settings, or uninstalling the app,
removes this data. Android backup is on for the app: if backup to your Google
Account is on for your device, the backup and transfers to a new device can
include your progress, and backups may keep earlier copies until they are
replaced or deleted.

<!-- Verified from: platform/android/app/src/main/AndroidManifest.xml [android:allowBackup="true"] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_removing_body] -->
<!-- Verified from: docs/PRIVACY.md [Plain Vim Practice for Android] -->

On iOS, the app has no iCloud sync, but your progress can be included in
iCloud Backup or a computer backup if you have backups turned on. Uninstalling
the app removes it from the device.

<!-- Verified from: dev-docs/store_listings/app_store.md [Store Details, iCloud backup] -->
<!-- Verified from: docs/PRIVACY.md [Removing data] -->

To clear your progress without uninstalling, use
[Reset All Progress](#reset-all-progress).

## Troubleshooting

| Symptom | Likely Cause | Resolution |
| --- | --- | --- |
| **Your data couldn't be opened** appears at startup | The app could not open its saved progress | Tap **Retry**. If it still fails, tap **Continue Without Saving** to use the app; your saved data stays on the device unchanged, but new changes are not saved while the orange banner shows. |
| The keyboard is gone in the emulator | The keyboard was hidden with the key-row button or by the system | Tap the practice text, or tap the keyboard button at the end of the key row. |
| Keys show under **Typed so far** but nothing happens | The command is not finished, such as `d` waiting for a motion | Finish the command, or press **Esc** to cancel it. |
| `:q` shows `E37: No write since last change` | The practice text has changes, and Vim protects unsaved work | Type `:w` first, or `:q!` to drop the changes. |
| A search or `:s` command finds no match for a pattern with special characters | The emulator matches plain text, not regular expressions | Search for the exact text instead. |
| A challenge's text matches the target but is not solved | You are still in Insert or Visual mode, or a command is half typed | Press **Esc** to return to Normal mode. |
| A challenge shows **Needs Full Access** | Challenges 4 to 14 need Full Access | Buy or restore Full Access; see [Unlock Full Access](#unlock-full-access). |
| **Checking Google Play…** or **Google Play is not available right now** on Android (**Checking the App Store…** or **The App Store is not available right now** on iOS) | The device is offline, or the store cannot be reached | Connect to the internet and open the **Full Access** screen again. |
| **No full access purchase was found** for your account | A different account is signed in to the store, or the purchase was refunded | Sign in to the store with the account you bought Full Access with, then tap **Restore Purchases**. |
| **Your purchase is waiting for approval** | The purchase needs payment or approval, such as from a family manager | Full Access starts once the store approves the purchase. |
| **Needs Review** says **Nothing to review yet** | You have not missed enough quiz questions on any command | Take quizzes on other choices first; commands you keep missing appear here. |
| **No email app was found. Use Open contact form instead.** in **Send Feedback** | No email app is set up on the device | Tap **Open contact form**, or write to <feedback@plaintxtoffice.com> from another device. |

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/root/StorageGate.kt -->
<!-- Verified from: platform/android/app/src/main/res/values/strings.xml [storage_failure_title, storage_failure_message, storage_failure_retry, storage_failure_continue, storage_failure_banner, full_access_notice_not_found, full_access_notice_pending] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_checking, emulator_unlock_unavailable, emulator_challenge_locked] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_feedback_no_email_app] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/vim/VimEngine.kt [E37, plain-text patterns] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Challenge.kt [ChallengeRun.isSolved] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/UnlockView.swift -->
<!-- Verified from: platform/ios/plain-vim-practice/StorageRecovery.swift -->

## FAQ

### Do I need an internet connection?

No. Everything works offline except buying or restoring Full Access, which
uses the store.

<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_services_body] -->

### Does the emulator run Vim?

No. It is a small Vim-style editor written for this app, and it contains no
Vim code. It edits a practice text in memory and never opens or saves files on
your device.

<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_privacy_about] -->

### What does Full Access add?

It opens challenges 4 to 14. Everything else is the same without it.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_feature_footer] -->

### Is Full Access a subscription?

No. It is a one-time purchase that stays with your store account and works
offline.

<!-- Verified from: platform/android/app/src/main/res/values/strings_emulator.xml [emulator_unlock_footer] -->

### Does the app collect my data?

No. It has no account, analytics, advertising, or tracking. Your progress stays
on your device, and a feedback email is sent only if you send it yourself.

<!-- Verified from: docs/PRIVACY.md [Summary] -->

### Why does my typed answer count as wrong?

Typed answers are case sensitive, as in Vim: `D` is not `d`. Check the case of
each letter.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/domain/Command.kt [Command.matches] -->

## Feedback

Send bug reports and feature requests by email to
<feedback@plaintxtoffice.com>, or through the contact page at
<https://plaintxtoffice.com/contact/>.

In the app, **Send Feedback** offers three choices:

- **Report a bug** and **Request a feature** open a draft in your email app,
  addressed to Plain Text Office, with your app version, system version, and
  device model filled in.
- **Open contact form** opens the contact page in your browser.

The draft never includes your learned commands, quiz answers, or progress.
Nothing is sent unless you send it.

To open it, tap **Send Feedback** on the **Home** tab, or in the **Docs** tab
choose **Guides** and tap **Send Feedback** under **About**.

<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/feedback/FeedbackIntents.kt [FEEDBACK_ADDRESS, CONTACT_URL, deviceSummary] -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/docs/FeedbackScreen.kt -->
<!-- Verified from: platform/android/app/src/main/kotlin/com/plaintxtoffice/plainvimpractice/feature/home/HomeScreen.kt [FeedbackPill] -->
<!-- Verified from: platform/android/app/src/main/res/values/strings_docs.xml [docs_feedback_how, docs_feedback_privacy] -->
<!-- Verified from: platform/ios/plain-vim-practice/Feedback.swift [address, contactURL] -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/HomeView.swift -->
<!-- Verified from: platform/ios/plain-vim-practice/Views/DocsView.swift -->

## Glossary

| Term | Meaning |
| --- | --- |
| Base plan | What the app includes without a purchase: the commands, guides, quizzes, key combos, emulator, and the first three challenges |
| Command line | The line at the bottom of the emulator where `:`, `/`, and `?` commands are typed |
| Full Access | The optional one-time purchase that opens all 14 challenges |
| Insert mode | The mode where keys type text; **Esc** leaves it |
| Key combo | Several keys typed together to do one editing task, such as `daw` |
| Motion | Keys that move the cursor, such as `w` or `$`, and that tell an operator how far to act |
| Normal mode | Vim's starting mode, where every key is a command |
| Operator | A command that acts on text, such as `d` (delete), `c` (change), or `y` (yank) |
| Par | The number of keys in the app's own answer to a challenge |
| Register | Where yanked or deleted text is kept for pasting; the emulator has one |
| Text object | A whole thing, such as a word or the inside of quotes, named with `i` or `a`, as in `ciw` |
| Visual mode | The mode for selecting text before acting on it |
| Yank | Vim's word for copy |
