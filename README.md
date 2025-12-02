# Skribbl.io Word Solver

Tampermonkey userscript that suggests **German** words for Skribbl.io by filtering a large word list based on the current hint pattern.

## 🚀 Features

- **Smart pattern matching** – filters words based on the Skribbl.io hint layout
- **Wildcard support** – `_` is treated as an unknown letter
- **Multi‑word & hyphen support** – handles phrases and compound words
- **Real‑time updates** – suggestions refresh as new letters appear
- **Click‑to‑type** – insert a suggestion into the chat with one click
- **Minimal UI** – small, non‑intrusive overlay

## 📦 Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/).
2. Open `Skript.js` in this repository.
3. Copy the entire file content.
4. Create a new userscript in Tampermonkey.
5. Paste the copied code and save.
6. Open [skribbl.io](https://skribbl.io/) – the script activates automatically on the page.

## 🎯 How It Works

The script matches all words in the German word list against the current hint:

- `_` → unknown letter (wildcard)
- `-` → hyphen inside compound words
- space (` `) → space between words
- multi‑word hints → handled via segment lengths

Matching candidates are displayed in an overlay where you can click them to type them into the chat.

## 📁 Project Structure

- `Skript.js` – production‑ready Tampermonkey userscript
- `src/GermanWordList.txt` – German word list used by the script
- `src/TestWords.txt` – test entries for development
- `src/Hints_format.html` – reference of the hint DOM structure used for parsing

## 🔧 Compatibility

- **Browsers**: Chrome, Firefox, Edge, Safari (with Tampermonkey)
- **Site**: Official Skribbl.io
- **Dependencies**: none besides Tampermonkey

## ⚡ Usage

1. Join any Skribbl.io lobby.
2. When it is your turn to guess, the script automatically reads the hint.
3. Suggested words are shown in the overlay.
4. Click a word to send it into the guess field.
5. As more letters are revealed, the suggestions update automatically.

## 🛠️ Technical Details

- **Author**: 062Leo
- **Current language support**: German word list, English UI
- **Planned languages**: English, Spanish, French (coming in future releases)
- **Implementation**: pattern‑based filtering with caching in plain JavaScript (no external libraries)

## 🤝 Contributing

Contributions are very welcome:

- improve or extend the word lists (starting with German)
- help add support for English, Spanish, and French
- report bugs or suggest improvements to the UI/UX

Feel free to open issues or pull requests.

## 📝 License

MIT License – free to use, modify, and share.

---

**Note:** For educational and entertainment purposes only. Please use responsibly and respect fair‑play rules.
