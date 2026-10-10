# Grundkenntnistest Zürich · practice deck

An unofficial practice page for the Canton of Zürich naturalisation knowledge test (*Kantonaler Grundkenntnistest im Einbürgerungsverfahren*): all 350 questions from the canton's official catalogue, in German, with English translations.

**Open it:** https://pepeenr.github.io/einburgerung-zuri/

## Using it

- Hover over a question to read it in English, or switch on **English inline** to show every translation (the way to go on a phone).
- The ⓘ icon on each card shows the question number, topic, PDF page and how often you got it wrong.
- Tick the correct answer and the question disappears. A wrong answer turns red and puts the question on the *To review* list, where it stays until you get it right on the first try.
- **Rapid fire** (button in the toolbar) shows your unfinished questions one at a time, full screen. When it starts, press any four keys, one after the other, to choose your own answer keys for a, b, c and d (Backspace undoes the last one); they stay the same until you leave. **Space** skips, **Esc** exits. On a touch screen you just tap. A right answer moves on at once; a wrong one turns red and you try again, with the same scoring as the list. It drills whatever the list is set to: the current topic and level filters, the current order, and the *To review* list when that tab is open. At the end you can drill just the ones you missed.
- Show the questions in PDF order or shuffled, filter by topic or by level (Bund, Kanton, Gemeinde), and optionally shuffle the answers.
- Progress is stored in your browser (localStorage), so each browser and device keeps its own.

## Editing

The whole app is one self-contained file, `index.html`: markup, styles, script, the question data and the images. There is no build step; GitHub Pages serves the file as it is.

Each question is one line in the `gkt-data` block. Search for `"i":123,` to find question 123:

| Field | Meaning |
|---|---|
| `q`, `o` | question and answers in German, as in the PDF |
| `qe`, `oe` | English translations |
| `a` | index of the correct answer (0 = a) |
| `p` | page in the PDF |

## Source

Questions and answers: «Kantonaler Grundkenntnistest im Einbürgerungsverfahren», Kanton Zürich, Direktion der Justiz und des Innern, Gemeindeamt. Maps © BFS. This project is not affiliated with the canton, and the English translations are unofficial.
