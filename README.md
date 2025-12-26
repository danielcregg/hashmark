# #️⃣ HashMark
> **The zero-dependency, serverless markdown editor that lives in your URL.**

HashMark is a powerful, feature-rich markdown editor that runs entirely in your browser. It uses the URL hash to store your document, meaning you can share "files" just by sending a link. No database, no accounts, no servers—just you and the client.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://danielcregg.github.io/hashmark/)
[![GitHub Pages](https://img.shields.io/badge/hosted-GitHub%20Pages-blue)](https://danielcregg.github.io/hashmark/)
[![No Backend](https://img.shields.io/badge/backend-none-orange)](https://danielcregg.github.io/hashmark/)

**🚀 Try it now:** [https://danielcregg.github.io/hashmark/](https://danielcregg.github.io/hashmark/)

---

## ✨ Features

### Editor & Preview
| Feature | Description |
|---------|-------------|
| 📝 **Full Markdown** | Complete GitHub-Flavored Markdown (GFM) support |
| 👁️ **Live Preview** | Real-time rendering as you type |
| 🔄 **Three View Modes** | Edit, Split, or Preview modes |
| 💾 **Auto-Save** | Changes saved automatically with visual indicator |
| 📊 **Word Count** | Live word and character count in status bar |

### Formatting Toolbar (Sidebar)
| Button | Function | Shortcut |
|--------|----------|----------|
| **B** | Bold text | `Ctrl+B` |
| *I* | Italic text | `Ctrl+I` |
| `</>` | Inline code | — |
| 🔗 | Insert link | `Ctrl+K` |
| H1/H2/H3 | Headings | — |
| • / 1. / ☐ | Lists (bullet, numbered, task) | — |
| 🖼️ | Insert image | — |
| ▦ | Insert table | — |
| " | Blockquote | — |
| ― | Horizontal rule | — |
| 📊 | **Mermaid diagrams** (8 templates) | — |
| { } | **Code blocks** (16 languages) | — |

### Diagram Support
Click the **📊 Diagram** button to insert pre-built templates:
- 🔀 Flowchart
- ↔️ Sequence Diagram
- 📦 Class Diagram
- 🔄 State Diagram
- 🗃️ ER Diagram
- 📅 Gantt Chart
- 🥧 Pie Chart
- 🧠 Mind Map

### Code Block Support
Click the **{ } Code** button to insert syntax-highlighted blocks:
- JavaScript, TypeScript, Python, Java
- C, C++, C#, Go, Rust
- HTML, CSS, SQL, Bash, JSON
- Ruby, PHP

### Advanced Rendering
| Feature | Example |
|---------|---------|
| **Math Equations** | `$E = mc^2$` or `$$\sum_{i=1}^n x_i$$` |
| **Syntax Highlighting** | Automatic for 180+ languages |
| **Emoji Shortcodes** | `:smile:` → 😄, `:rocket:` → 🚀 |
| **Mermaid Diagrams** | Lazy-loaded for performance |

### Toolbar Actions
| Button | Function |
|--------|----------|
| ↶ / ↷ | Undo / Redo (`Ctrl+Z` / `Ctrl+Y`) |
| ☀️ 🌙 📜 | Theme toggle (Light / Dark / Sepia) |
| 📄 New | Open fresh document in new tab |
| 💾 | Download as `.md` file |
| 📋 | Copy rendered HTML |
| 🖨️ | Print / Export to PDF |
| 📱 | Generate QR code for sharing |
| 📤 | Share URL (copy to clipboard) |
| ⛶ | Fullscreen mode (`F11`) |

### Sharing & Collaboration
- 🔗 **URL-based sharing** — Document encoded in URL hash
- 🗜️ **Smart compression** — Deflate compression for compact URLs
- 📱 **QR Code generation** — Scan to share on mobile
- 📤 **Native sharing** — Uses mobile share sheet when available
- 💾 **Dual persistence** — Stored in localStorage AND URL

### Theming
Three beautiful themes that persist across sessions:
- ☀️ **Light** — Clean, bright interface
- 🌙 **Dark** — Easy on the eyes
- 📜 **Sepia** — Warm, paper-like feel

---

## 🚀 Quick Start

1. **Open** the editor at [danielcregg.github.io/hashmark](https://danielcregg.github.io/hashmark/)
2. **Write** your markdown in the editor pane
3. **Preview** using Split or Preview mode
4. **Share** by clicking 📤 Share or 📱 QR Code
5. **Export** as `.md`, HTML, or PDF

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+B` | Bold |
| `Ctrl+I` | Italic |
| `Ctrl+K` | Insert link |
| `Ctrl+S` | Save |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` / `Ctrl+Shift+Z` | Redo |
| `Tab` | Insert 2 spaces |
| `F11` | Toggle fullscreen |
| `Escape` | Exit fullscreen |

---

## 📖 Markdown Support

### Text Formatting
```markdown
**Bold**, *italic*, ***bold italic***
~~Strikethrough~~, `inline code`
```

### Headings
```markdown
# H1  ## H2  ### H3  #### H4  ##### H5  ###### H6
```

### Lists
```markdown
- Bullet item
1. Numbered item
- [ ] Task item
- [x] Completed task
```

### Links & Images
```markdown
[Link text](https://example.com)
![Alt text](image.png)
```

### Code Blocks
````markdown
```javascript
console.log('Hello, World!');
```
````

### Tables
```markdown
| Header 1 | Header 2 |
|----------|----------|
| Cell 1   | Cell 2   |
```

### Math (KaTeX)
```markdown
Inline: $E = mc^2$
Block: $$\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}$$
```

### Mermaid Diagrams
````markdown
```mermaid
graph TD
    A[Start] --> B{Decision}
    B -->|Yes| C[Action]
    B -->|No| D[End]
```
````

### Emoji Shortcodes
```markdown
:smile: :rocket: :fire: :thumbsup: :heart:
```

---

## 🛠️ Technical Details

| Component | Technology |
|-----------|------------|
| Markdown Parser | [Marked.js](https://marked.js.org/) v11.1.1 |
| Syntax Highlighting | [Highlight.js](https://highlightjs.org/) v11.9.0 |
| Math Rendering | [KaTeX](https://katex.org/) v0.16.9 |
| Diagrams | [Mermaid](https://mermaid.js.org/) v10 (lazy-loaded) |
| QR Codes | [QRious](https://github.com/neocotic/qrious) v4.0.2 |
| Compression | Native CompressionStream API (deflate-raw) |
| Storage | localStorage + URL hash |
| Hosting | GitHub Pages (static) |

---

## 💡 Pro Tips

- Start your document with `# Title` to set the browser tab title
- Use **Split** mode for the best editing experience
- Your theme and view mode preferences are remembered
- Click outside modals to close them
- QR codes work offline once generated
- Long documents? The URL still works—compression is efficient!

---

## 📋 Use Cases

- 📚 Technical documentation
- 📰 Blog posts and articles
- 📋 Meeting notes and agendas
- 📦 Project README files
- 📓 Personal journals
- 💻 Code tutorials
- ✅ Quick notes and checklists
- 📊 Diagrams and flowcharts

---

## 🤝 Contributing

Contributions are welcome! This is a single-file application—all code lives in `index.html`.

---

## 📄 License

MIT License — feel free to use, modify, and share.

---

<p align="center">
  Made with ❤️ and JavaScript<br>
  <a href="https://danielcregg.github.io/hashmark/">Try it now →</a>
</p>
