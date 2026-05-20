# Morse Academy

> **Learn Morse code interactively with a visual dichotomic schema.**
> Tap the telegraph key, follow the lit-up path, decode letters in real time.

**🛠 Full toolkit (translator, audio player, practice trainer, alphabet reference):** https://morse.megolo.com/

---

## ✨ Features

- 📊 **Visual schema** — every letter is a path on a dichotomic tree (left = dot, right = dash)
- 🔊 **Real telegraph tone** — 700 Hz sine wave, plays while you hold the key
- ⌨️ **Keyboard support** — Space = signal, Enter = confirm, Backspace = delete
- 📱 **Mobile-friendly** — works as a tap-and-hold telegraph key on any phone
- 🚀 **Zero dependencies** — one HTML file, no build step, no tracking
- 🔌 **Offline-ready** — works without an internet connection after first load

## 🎯 How it works

Morse code is naturally **dichotomic**: each signal is either a dot (`•`) or a dash (`—`). The schema turns that structure into a tree. Starting at the root:

- A **short tap** (< 200 ms) sends a **dot** → branch left
- A **long hold** (≥ 200 ms) sends a **dash** → branch right

After 1 second of inactivity the current letter is added automatically. The most common English letters (E, T, A, I, N, M, S, O) sit closest to the root because they have the shortest codes.

### Quick examples

| Letter | Code | Path |
|--------|------|------|
| E | `•` | one dot |
| T | `—` | one dash |
| A | `•—` | dot, dash |
| N | `—•` | dash, dot |
| SOS | `••• ——— •••` | the international distress signal |

## 🚀 Run locally

It's a single static file — just open it in a browser.

```bash
git clone https://github.com/metastaa/morse-academy.git
cd morse-academy
open index.html        # macOS
# or: xdg-open index.html   # Linux
# or just double-click the file
```


## 🧭 Roadmap / Want more?

This repo is intentionally minimal — a clean, focused way to learn the alphabet via the schema. If you want the full Morse code workbench:

👉 **[morse.megolo.com](https://morse.megolo.com/)** has:
- Bidirectional **text ↔ Morse translator**
- **Audio player** with adjustable WPM
- **Practice trainer** with stats (correct / wrong / streak)
- Complete **alphabet reference** (letters, numbers, punctuation)
- Dark mode, multi-language UI

## 🙏 Credits

Schema layout inspired by the classic *Morse Code Receive Decoder Chart* by **Dave Nathanson, KG6ZJO**.

## 📄 License

[MIT](LICENSE) — do whatever you want, attribution appreciated.
