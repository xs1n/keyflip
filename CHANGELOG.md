# What's new in KeyFlip

[Русская версия](CHANGELOG.ru.md)

## 1.0 — October 23, 2026

First release of KeyFlip, a free keyboard layout auto-switcher for macOS.

**Layout fixing**
- A word typed in the wrong layout is fixed after a space, Return, Tab or punctuation, and the layout switches by itself: `ghbdtn` → «привет», `руддщ` → `hello`.
- A short word before a word in the other language is fixed too, also after switching the layout by hand: «d меню» → «в меню», «f не» → «а не», «vs с тобой» → «мы с тобой». Real short words stay: «в USB», «на GitHub», “a day”.
- Ordinary words, abbreviations and names (ok, zoom, git, docker, «спс») are left alone.

**By hand**
- ⌥ Option (press and release) flips the last word — the whole thing up to the space, digits included (`чы1т` → `xs1n`) — or the selected text. Left, right or either Option.
- Double Shift right after a fix undoes it.

**Small typos**
- Particles: «почемуто» → «почему-то», «гденибудь» → «где-нибудь», «коекто» → «кое-кто», «кембы» → «кем бы».
- Glued words: «сонатуБаха» → «сонату Баха».
- Punctuation typed in the Russian layout: «пирогб» → «пирог,». Letter case: «ПРивет» → «Привет», «пРИВЕТ» → «Привет» (and Caps Lock goes off).

**Left alone**
- E-mails, sites and links (`name@gmail.com`, `https://…`), passwords, brands and abbreviations (iPhone, YouTube, ООО, PDF). An abbreviation typed in the wrong layout is recognised: `jjj` → «ООО».
- Code editors, terminals and games are excluded out of the box; add any other app.

**Dictionaries and learning**
- “My words” (nicknames, names, slang) and “Learned” — KeyFlip learns when you undo a fix, erase it and type the same again, or flip a word it missed.
- Instant search in either layout, right-click to delete, export and import of both dictionaries in one file.

**The app**
- Menu bar icon and a settings window: General, Dictionaries, Exclusions, About.
- A welcome window on first launch shows how to allow keyboard access.
- Updates itself: once a day it checks GitHub for a new version and installs it when you click Install.
- Click sound on fixes, open at login, no account and no analytics.
