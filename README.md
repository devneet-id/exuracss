# E X U R A . C S S

**Exura.css** is a modern, semantic-first CSS framework that reimagines how you style the web.  
Forget the noise of long class names — Exura brings a **cleaner**, more **declarative** approach using **attribute-based styling**.

Designed for simplicity and scalability, Exura.css helps you build beautiful interfaces with clean, readable HTML.

## ✨ Key Features

- 🌀 **Attribute-Based Styling**  
  Use custom HTML attributes instead of traditional classes for maximum clarity.

- 🧼 **Cleaner Markup**  
  Eliminate clutter with semantic, expressive HTML.

- ⚡ **Lightweight & Fast**  
  Built for performance — no heavy resets or bloated stylesheets.

- 🔧 **Fully Customizable**  
  Adapt Exura to your own design system with ease.

## 🔍 Example

```html
<!-- component -->
<button button="primary">Click Me</button>

<!-- intuitive grid with flex & width -->
<div flex="wrap">
  <div size="w-1/2">50%</div>
  <div size="w-1/2">50%</div>
</div>
```

Simple, readable, and powerful — that’s the EXURA way.
Perfect for developers who value clarity, maintainability, and innovation in frontend development. ✨



## 🛠️ BUILD WITH RUNE

**Exura** uses the **Rune** build engine.  
Before getting started, we recommend reading the official documentation here:  
👉 <https://github.com/devneet-id/rune>

Although in most cases you can simply run the available `build` commands, understanding the **Rune structure** will help you better track and manage post-processing tasks more efficiently.

Requirements, Make sure you have:
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


## 🎯 G O A L
Exura will:
- Be fully integrated with **Rune** as its built-in build engine.

- Provide a targeted **preprocessing system**, similar to Tailwind CSS, but built entirely within the Rune ecosystem.

- Offer **unlimited flexibility** — supporting modern styling via class, attribute, or even the latest CSS features.

- Stay committed to **never becoming a burden** or bottleneck for developers.

Instead, Exura exists to empower, not to interrupt