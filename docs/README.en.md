# 🌐 Custom Google Translate Language Switcher Widget

> A lightweight, embeddable language switcher using Google Translate

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

* designed for **blog platforms with HTML support** (e.g., Tistory, GitHub Pages, WordPress).

* Provide a truly multilingual experience on your blog – with just one click and without any server-side configuration.

---

## 📦 Installation (General)

1. Add the contents of `widget.html` to any HTML-injectable section
2. Place it inside a sidebar, footer, or header area
3. Customize colors, layout, or language set as needed
4. Share a link with `?lang=xx` to allow users to land on a pre-translated view

> Works with Tistory, GitHub Pages, WordPress, and most CMS platforms that allow raw HTML/JS insertion.

---

## ✨ Key Features

* 🏳️ Flag-based language selector with `active state`
* 💾 Persistent language memory (LocalStorage)
* 🌐 `?lang=xx` URL parameter support
* 🔁 SPA compatibility (pushState / replaceState)
* 🎨 Easy UI customization with `Tailwind & CSS variables`
* 📦 CDN-based flag icons via [flagcdn.com](https://flagcdn.com)

---

## 🌏 Seamless Experience for Visitors

* Visitors can enter your site using a link like `?lang=ja` or `?lang=zh-CN`
* Translation is applied **automatically** on arrival, with no user action required
* Language preference is **persisted**, so users can **browse naturally**
  – as if the site were originally written in their language

<br/>

> 📌 **Example**: <br/>
> 👉 `https://yourblog.com/?lang=ja`

→ Instantly loads the Japanese version <br/>
→ No need to touch a language button <br/>
→ Feels like a native Japanese blog from start to finish

---

## 💻 Compatible Blog Platforms

* ✅ Tistory (via HTML banner plugin)
* ✅ GitHub Pages, Jekyll, Hugo (static sites)
* ✅ Self-hosted WordPress or CMS with HTML widget support

⚠️ Not compatible with platforms that **do not allow `<script>` or custom HTML**, such as Notion, Brunch, or Velog.

---

## 💡 Why Use This?

| Feature                              | `element.js` Default | `GTranslate` Widget | This Custom Widget      |
| ------------------------------------ | -------------------- | ------------------- | ----------------------- |
| `?lang=xx` support                   | ❌ No                 | ✅ Yes               | ✅ Yes                   |
| Language setting persistence         | ❌ Unstable           | ✅ Yes               | ✅ LocalStorage-based    |
| Visual language state indicator      | ❌ No                 | ❌ Limited           | ✅ Flag button active UI |
| UI customization                     | ❌ Minimal            | ❌ Difficult         | ✅ Tailwind + CSS vars   |
| SPA support (pushState/replaceState) | ❌ No                 | ❌ No                | ✅ Yes                   |
| Flag-based button UI                 | ❌ Dropdown only      | ✅ (iframe-based)    | ✅ Fully customizable    |
| Uses Google Translate engine         | ✅ Yes                | ✅ Yes               | ✅ Yes (indirectly)      |

> This widget is built on top of `element.js`, a legacy Google Translate script.
> Though undocumented, it's stable enough for lightweight UI integration.

> Future versions may support `GTranslate`-based implementation for more robust translation behavior.

---

## 🚧 Limitations

* Slight **delay** in initial translation on slower networks
* `element.js` is an **undocumented legacy script**, with behavior possibly changing in the future
* **SPA translation edge cases** may still occur – feel free to open Issues or submit PRs

---

## 🙌 Contributions Welcome

You’re welcome to:

* Add new language buttons
* Improve accessibility
* Adapt it to other blog/CMS platforms
* Share beautiful usage examples or themes!

Pull requests and suggestions are always appreciated ❤️

---

## 📁 Files

* `public/index.html` – Fully functional embeddable code
* `docs/README.ko.md` – Korean documentation
* `docs/README.en.md` – English version (this file)
