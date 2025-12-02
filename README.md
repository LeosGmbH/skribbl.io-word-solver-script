# Skribbl.io Word Solver

A Tampermonkey userscript that provides intelligent word suggestions for Skribbl.io by filtering a comprehensive German word list based on hint patterns.

## 🚀 Features

- **Smart Pattern Matching** - Filters words based on Skribbl.io hint structure
- **Wildcard Support** - Underscore (_) treated as unknown letters
- **Multi-word Handling** - Supports phrases, hyphens, and compound words
- **Real-time Updates** - Automatically refines suggestions as hints reveal
- **Click-to-Type** - Instant word input with a single click
- **Clean Interface** - Non-intrusive overlay design

## 📦 Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/)
2. Copy `Fertiges skript.js` 
3. Create new userscript in Tampermonkey
4. Paste code and save
5. Visit Skribbl.io - script activates automatically

## 🎯 How It Works

The script analyzes hint patterns:
- `_` = unknown letter (wildcard)
- `-` = hyphen in compound words  
- ` ` = space between words
- Numbers = word lengths for multi-word answers

## 📁 Files

- `Fertiges skript.js` - Production-ready userscript
- `wordlistFertig.txt` - German word database (4,000+ words)
- `Hints_format.html` - HTML structure reference
- `testing.js` - Development version
- `obfuscated.js` - Minified version

## 🔧 Compatibility

- **Browsers**: Chrome, Firefox, Edge, Safari
- **Site**: Skribbl.io official
- **Dependencies**: None (Tampermonkey only)

## 📊 Word List Stats

- **4,000+ German words** - From 2-letter to multi-word phrases
- **Categories**: Objects, animals, places, brands, characters, concepts
- **Format**: JSON array for easy integration
- **Updates**: Comprehensive German vocabulary

## ⚡ Usage

1. Join any Skribbl.io game
2. When guessing, script detects hint pattern automatically  
3. View filtered suggestions in overlay
4. Click any word to input it instantly
5. Suggestions update as more hints appear

## 🎮 Game Integration

- **Automatic Detection** - No manual setup required
- **Non-intrusive** - Clean overlay doesn't block gameplay
- **Performance** - Optimized filtering with caching
- **Fair Play** - Enhances, doesn't automate completely

## 🛠️ Technical Details

- **Version**: 4.6
- **Author**: 062Leo
- **Language**: German word list with English interface
- **Pattern Algorithm**: Advanced regex matching with caching
- **UI Framework**: Pure JavaScript/CSS (no external dependencies)

## 📝 License

MIT License - Open source, free to use and modify

---

**Note**: For educational and entertainment purposes. Use responsibly and respect fair play guidelines.
