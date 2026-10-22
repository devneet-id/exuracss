# E X U R A . C S S

**Exura.css** is a semantic-first CSS framework: you style with **attributes**, not long class names.
Part of the **Exura series** — the power of a modern CSS framework in a single, super-light stylesheet.

```html
<button button="primary">Save</button>
```

## ✨ Key Features

- 🌀 **Attribute-based styling** — every concern has its own attribute: `button`, `card`, `flex`, `size`, `ring`, `text`, `list`, `table`, `misc`.
- 🧼 **Readable markup** — values read like a sentence: `flex="wrap j:between a:middle"`, `size="w:1/2 p:2"`.
- 📱 **Responsive by prefix** — `md:size="w:1/3"` applies from the `md` breakpoint up.
- 🌗 **Dark mode by color balancing** — one palette; every shade (`primary-1` … `primary-10`) is a transparent tint that blends with the background. Add `dark` to `<body>`, nothing else changes.
- 🎨 **One token file** — colors, text sizes, breakpoints and spacing live in `exura.json`.
- 😀 **Clip icons** — emoji icons as attributes (`<i clip="rocket animate"></i>`) in the separate `exura-clip.css`.

## 📦 Install

Use the built files from `dist/` — no build step needed:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devneet-id/exuracss@1.x/dist/exura.min.css">
<!-- optional: emoji icons -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devneet-id/exuracss@1.x/dist/exura-clip.css">
```

## 🔍 Example

```html
<body dark>

  <div container>
    <div flex="wrap j:between a:middle">
      <div size="w:full" md:size="w:1/2">
        <div card="primary:2" ring="b:full b:primary-5" size="p:2">
          <span text="h4 bold primary">Exura</span>
          <p text="default">Tinted card that balances on light and dark.</p>
        </div>
      </div>
      <button button="primary">Click Me</button>
    </div>
  </div>

</body>
```

| Attribute | Examples |
|---|---|
| `button` | `primary`, `secondary`, `dark`, `none` |
| `card` | `primary`, `light`, `primary:3` (shade 1–10) |
| `flex` | `wrap`, `d:column`, `j:between`, `a:middle`, `1` |
| `size` | `w:1/2`, `w:full`, `h:1/4`, `p:2`, `mx:auto`, `pt:1.5` |
| `ring` | `b:full`, `b:dashed`, `b:primary-5`, `o:full`, `s:full s:lg` |
| `text` | `h1`…`h6`, `display:1`…`4`, `bold`, `center`, `primary`, `ellipsis` |
| `misc` | `d:none`, `p:sticky`, `z:3`, `ws:nowrap` |
| `list` / `table` | `ring:y`, `dir:x` / `ring`, `ring:x`, `ring:y` |

## 🧩 The Exura Series

Exura mirrors a modern CSS / JS / PHP framework — at a fraction of the weight, without losing the abilities of a framework.

| Package | Focus | Repository |
|---|---|---|
| **exuracss** | modern semantic styling | [devneet-id/exuracss](https://github.com/devneet-id/exuracss) |
| **exurajs** | modern reactive JavaScript | [devneet-id/exurajs](https://github.com/devneet-id/exurajs) |
| **exuraphp** | modern HTTP API endpoints | [devneet-id/exuraphp](https://github.com/devneet-id/exuraphp) |

## 🛠️ Shaped with Rune

This project is shaped with **Rune** — a lore-driven, modular concept beneath PHP that responds to development rather than dictating it.  
Its runite, `cast`, holds the casts that turn `src/` into `dist/`.  
👉 <https://github.com/devneet-id/rune>

You can simply run the casts below; knowing how a runite works helps when you want to shape your own.

Requirements:
- **Composer** installed
- **PHP version 8.1+**

Then run this command:

```bash
composer install
```

The runite of this project is `cast`. To view its main screen (all casts with notes):
```shell
php cast
```

To build the project:
```shell
php cast build
php cast build --min=true
```

Build the emoji icon set (`dist/exura-clip.css`):
```shell
php cast build-clip
```

Version (stored in the runite itself as `const VERSION`, applied on build):
```shell
php cast version
php cast version --up            # 1.0.0 -> 1.0.1  (--up=minor | major | release)
php cast version --pre           # 1.0.1 -> 1.0.1-dev  (--pre=beta.1)
php cast version --set=1.0.0
```

## 🎯 Goal

Exura.css will:

- Generate **only what you use** — an on-demand cast that scans your HTML, in the spirit of utility-first frameworks.
- Speak **one grammar** across all attributes, so every value can be combined the same way.
- Keep **color balancing** at its core — one palette that works on any background.
- Stay **light** and never become a burden for the developer.

Exura.css exists to empower, not to interrupt.
