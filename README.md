# 📝 Text Manager

A clean, fully client-side text editor and organizer that runs entirely in the browser — no server, no account, no internet required after loading. Built as a single HTML file, perfect for hosting on GitHub Pages.

---

## ✨ Features

- **Create, edit, rename, and delete** named text entries
- **Auto-save** — changes are saved automatically after 2 seconds of inactivity
- **Persistent storage** — all texts are stored in `localStorage` and survive page refreshes
- **Syntax modes** — Plain Text, Markdown, HTML, JavaScript, CSS, JSON
- **Live Markdown preview** — side-by-side editor and rendered preview
- **Find & Replace** — search within a text with match counter and prev/next navigation
- **Import files** — load `.txt`, `.md`, or `.json` files from your device
- **Export / Download** — save any text as `.txt`, `.md`, `.json`, or `.html`
- **Copy to clipboard** — one-click copy of the full text
- **Line numbers** — synchronized scrolling line number gutter
- **Search** — filter your saved texts by title or content with live highlighting
- **Dark & light theme** — manual toggle with system preference detection; choice is remembered
- **Storage usage indicator** — shows how much of your ~5MB localStorage quota is in use
- **Keyboard shortcuts** — fast workflow without reaching for the mouse
- **Fully responsive** — works on desktop and mobile

---

## 🚀 Usage

### GitHub Pages

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Set source to your `main` branch, root folder
4. Visit `[https://yourusername.github.io/your-repo-name/Texts_Manager.html](https://nuhbodyok.github.io/txts/)`

### Local

Just open `Texts_Manager.html` in any modern browser — no build step, no dependencies.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+S` | Save current text |
| `Ctrl+D` | Download current text |
| `Ctrl+N` | Focus new text title field |
| `Ctrl+F` | Open Find bar |
| `Ctrl+H` | Open Find & Replace bar |
| `Ctrl+P` | Toggle Markdown preview |
| `Tab` | Indent line or selection |
| `Shift+Tab` | Unindent line or selection |
| `Esc` | Close modal or Find bar |

---

## 📁 File Import & Export

**Import** supports:
- `.txt` — loaded as plain text
- `.md` — loaded with Markdown syntax mode
- `.json` — if the file contains `{ "title": "...", "content": "..." }`, both fields are used; otherwise treated as plain text

**Export** formats:
- `.txt` — plain text
- `.md` — Markdown
- `.json` — structured object with title, content, timestamps, and syntax mode
- `.html` — raw HTML content

---

## 🗄️ Data Storage

All data is stored in your browser's `localStorage` under the key `text-manager-data`. Nothing is ever sent to a server.

- **Capacity:** ~5MB (browser-imposed localStorage limit)
- **Persistence:** Survives page refreshes and browser restarts
- **Portability:** Use the JSON export to back up or move your texts between devices

> ⚠️ Clearing your browser's site data will erase all saved texts. Export important texts regularly.

---

## 🛠️ Tech Stack

| Layer | Details |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 with custom properties (dark/light theming) |
| Logic | Vanilla JavaScript (ES6+) |
| Storage | Browser `localStorage` |
| Dependencies | None |

---

## 🌐 Browser Compatibility

Works in all modern browsers. No polyfills or build tools required.

| Browser | Supported |
|---|---|
| Chrome / Edge | ✅ |
| Firefox | ✅ |
| Safari | ✅ |
| Mobile browsers | ✅ |

---

## 📄 License

MIT — do whatever you want with it.
