# HashMark

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)

> **Note:** This repository is a fork of [antonmedv/textarea](https://github.com/antonmedv/textarea).

A zero-dependency, serverless Markdown editor that lives entirely in your URL. Write, preview, and share documents by simply sending a link -- no database, no accounts, no servers required.

**Live Demo:** [danielcregg.github.io/hashmark](https://danielcregg.github.io/hashmark/)

## Overview

HashMark is a feature-rich Markdown editor that runs entirely in the browser. It encodes your document into the URL hash using deflate compression, enabling you to share complete documents as links. It supports GitHub-Flavored Markdown, Mermaid diagrams, KaTeX math equations, syntax highlighting for 180+ languages, and multiple themes.

## Features

- **Full GFM Markdown** -- Complete GitHub-Flavored Markdown support with live preview
- **Three View Modes** -- Edit, Split, or Preview mode for flexible editing
- **URL-Based Storage** -- Documents encoded in the URL hash using deflate compression
- **Mermaid Diagrams** -- Eight diagram templates including flowcharts, sequence, class, state, ER, Gantt, pie, and mind maps
- **Math Equations** -- KaTeX rendering for inline (`$...$`) and block (`$$...$$`) math
- **Syntax Highlighting** -- Highlight.js support for 180+ languages with code block templates for 16 popular languages
- **Three Themes** -- Light, Dark, and Sepia themes that persist across sessions
- **Formatting Toolbar** -- Sidebar with bold, italic, headings, lists, tables, images, blockquotes, and more
- **Keyboard Shortcuts** -- `Ctrl+B` (bold), `Ctrl+I` (italic), `Ctrl+K` (link), `Ctrl+Z/Y` (undo/redo), `Tab` (indent)
- **Smart Editing** -- Auto-closing pairs, smart list continuation, block indent/dedent
- **QR Code Sharing** -- Generate QR codes for mobile sharing
- **Export Options** -- Download as `.md`, copy as HTML, or print/export to PDF
- **Dual Persistence** -- Stored in both localStorage and URL hash
- **Emoji Shortcodes** -- `:smile:`, `:rocket:`, `:fire:`, and more

## Prerequisites

- A modern web browser with JavaScript enabled
- No installation, server, or build tools required

## Getting Started

### Installation

No installation is needed. HashMark is a single-file static application.

To self-host, clone the repository and serve `index.html`:

```bash
git clone https://github.com/danielcregg/hashmark.git
cd hashmark
# Serve with any static file server, e.g.:
python -m http.server 8000
```

Alternatively, deploy directly to GitHub Pages.

### Usage

1. Open the editor at [danielcregg.github.io/hashmark](https://danielcregg.github.io/hashmark/)
2. Write your Markdown in the editor pane
3. Toggle between Edit, Split, or Preview modes
4. Share by clicking the Share button or generating a QR code
5. Export as `.md`, HTML, or PDF

**Keyboard Shortcuts:**

| Shortcut | Action |
|----------|--------|
| `Ctrl+B` | Bold |
| `Ctrl+I` | Italic |
| `Ctrl+K` | Insert link |
| `Ctrl+S` | Save |
| `Ctrl+Z` | Undo |
| `Ctrl+Y` | Redo |
| `Tab` | Insert 2 spaces |
| `F11` | Toggle fullscreen |

## Tech Stack

| Technology | Purpose |
|------------|---------|
| JavaScript | Core application logic |
| HTML5 | Single-file application structure |
| CSS3 | Theming and responsive layout |
| Marked.js | Markdown parsing (v11.1.1) |
| Highlight.js | Syntax highlighting (v11.9.0) |
| KaTeX | Math equation rendering (v0.16.9) |
| Mermaid | Diagram rendering (v10, lazy-loaded) |
| QRious | QR code generation (v4.0.2) |
| CompressionStream | Native deflate compression for URL encoding |
| GitHub Pages | Static hosting |

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
