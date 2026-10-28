<!-- ============================================================
     Profile README — built like a design handoff sheet.
     One column everywhere, so phones and desktops read the same.
     ============================================================ -->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:6C63FF,100:00C2A8&height=170&section=header&text=Eswar%20Varma%20Panumetcha&fontSize=40&fontColor=ffffff&desc=Frontend%20%26%20Mobile%20Engineer&descSize=18&descAlignY=80&animation=twinkling">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:C7C3FF,100:9FF3E8&height=170&section=header&text=Eswar%20Varma%20Panumetcha&fontSize=40&fontColor=2A2350&desc=Frontend%20%26%20Mobile%20Engineer&descSize=18&descAlignY=80" alt="Eswar Varma Panumetcha — Frontend & Mobile Engineer" width="100%">
</picture>

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&pause=900&color=6C63FF&center=true&vCenter=true&width=460&lines=UI+enhancement+track+%E2%80%94+Logray;UI+enhancement+track+%E2%80%94+JOYIZM;Design+systems+%C2%B7+motion+%C2%B7+accessibility;PROEDIT+%E2%80%94+local-first+mobile+video+editor;Home+widgets" alt="Currently shipping Logray and JOYIZM UI enhancements, and building PROEDIT, a local-first mobile video editor, plus home widgets" width="460" />

<br>

[![Email](https://img.shields.io/badge/Email-varmapanumetcha02%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:varmapanumetcha02@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-%2B91%209014832822-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/919014832822)
[![GitHub](https://img.shields.io/badge/GitHub-EswarVarma91-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EswarVarma91)

</div>

> [!NOTE]
> **Open handoff.** I take product screens that grew screen by screen and turn them into one consistent, reusable UI layer — shared components, honest states, motion that explains itself. Two tracks are live right now: **Logray** and **JOYIZM**. I'm also building **PROEDIT**, a local-first mobile video editor, and **home widgets**.

---

## 01 · 🎨 Logray — UI enhancement track

|  |  |
|:--|:--|
| **Status** | ● In build |
| **Scope** | Existing product screens → one reusable UI layer |
| **Craft** | Components · tokens · motion · accessibility · responsive |
| **Stack** | React · TypeScript · Ionic React · Capacitor |

Logray's interface grew feature by feature, so the job is consolidation: one component per job, one spacing and type scale, screens that behave the same at 360px and at 1440px. The product screens stay private — the approach doesn't.

| Before | After |
|:--|:--|
| Styled per screen | One component per job |
| Spacing eyeballed | Token scale |
| Blank jump on load | Skeletons + empty/error |
| Random tap targets | ≥44px, visible focus |
| “Works on my screen” | Phone → desktop checked |

- 🧩 **Component inventory first** — repeated blocks get pulled into one component with props, instead of a copy per screen.
- 📐 **Screen-by-screen refinement** — hierarchy, alignment and density brought in line with the rest of the product.
- ⚡ **Interaction polish** — transitions and loading feedback that explain what changed, not decoration.
- ♿ **Accessibility as a pass, not a hope** — contrast, focus order, keyboard paths and screen-reader labels verified.
- 📱 **Responsive by construction** — the same screen and the same logic from phone to desktop.

<!-- ============================================================
     Logray screenshot gallery — BLOCKED ON IMAGES.
     Add files to assets/logray/ (see the README in that folder), then
     delete the three comment lines below to publish the gallery.
     Replace the captions with what each screen actually shows.
     ============================================================

<p align="center">
  <img src="assets/logray/01-before.png" alt="Logray screen before the UI enhancement work" width="480">
  <br>
  <sub><b>Before</b> — screens styled one at a time</sub>
</p>

<p align="center">
  <img src="assets/logray/02-after.png" alt="The same Logray screen after the UI enhancement work" width="480">
  <br>
  <sub><b>After</b> — shared components, token-based spacing, real loading states</sub>
</p>

<p align="center">
  <img src="assets/logray/03-components.png" alt="Logray component library and design tokens" width="480">
  <br>
  <sub><b>System</b> — the component layer the screens are built from</sub>
</p>

-->

---

## 02 · PROEDIT — local-first mobile video editor

|  |  |
|:--|:--|
| **Status** | ● In build |
| **Project** | PROEDIT — Edit. Grade. Export. |
| **Platforms** | iOS 15+ and Android 7.0+ (minSdk 24) |
| **Stack** | Flutter · Cubits only · FFmpeg · SQLite |

PROEDIT is a complete, local-first mobile video editor. It uses a proxy-based editing workflow with a single-pass FFmpeg export graph, so scrubbing stays smooth on a phone while the final render always uses the original camera files.

| Area | What you get |
|:--|:--|
| Library | Multi-select import from Photos, the two bundled demo clips, or Pexels stock |
| Timeline | Multi-track video strip with drag-free trim handles, split, reorder, delete, undo/redo |
| Editing | Speed 0.25×–4×, 36 color looks + brightness/contrast/saturation, fit/fill framing, canvas colour, rotation/flip, text overlays with 9 presets + free drag placement, clip volume/mute |
| Finishing | Project fade-in and fade-out from black, covering text and PIP |
| Audio | Per-clip volume, background music import, fade in and automatic 1.5s outro fade |
| Transitions | Cut, dissolve, fade, slide, wipe, zoom, clamped to 45% of adjacent clips |
| PIP | Up to six picture-in-picture layers per project, each with 9 anchors, its own start time, size, opacity, volume and optional green/blue-screen backdrop removal |
| Merge | Two-clip side-by-side, stacked or overlay merge; overlay mode can key out a plain backdrop |
| Editing defaults | Persistent studio setup: export frame, resolution, fps and quality, plus default transition and length, clip framing, clip volume and project fades |
| Templates | 12 curated recipes plus an optional pack library; picking a template applies its filters, frame size, pacing, fades, titles and optional generated voice intro |
| Collage | 2, 4, 6, 8, 10 or 12 clips as side-by-side, stacked, feature or automatic grid; saved as a project and exported as one video |
| Stock | Optional Pexels video search; clips download, then follow the normal probe/proxy/import path |
| Export | 720p / 1080p / 4K, 16:9 / 9:16 / 1:1 / auto, 24/30/60 fps, draft/balanced/high, hardware H.264 when available |
| Export queue | Up to 10 jobs; Android keeps the render alive in a foreground service, iOS keeps the queue in-app |
| Sharing | Save to Photos, share sheet, or keep the file in the app export folder |
| Ads | Master toggle off by default, banners only on Gallery/Settings, one interstitial only after a successful export |

[🌐 GitHub repo →](https://github.com/EswarVarma91/video_editor)

---

## 03 · ✨ JOYIZM — UI enhancement track

|  |  |
|:--|:--|
| **Status** | ● In build |
| **Product** | Urban lifestyle membership — sport, wellness, meals, travel |
| **Scope** | iOS · Android · web, one design language |
| **Stack** | Next.js web · native apps · design system |

- 📱 **One experience across iOS, Android and web** — discover → book → pay → manage membership.
- 🧩 **Eight verticals in a single app**: events, meals, wellness, shop, deals, travel, activities, games.
- 🍽️ **Booking and redemption flows** — including the daily featured kitchen.
- 💳 **JOY Cash wallet** — balance, top-up and spend screens.
- 🧭 **Guest-first browsing** — see what's on nearby before signing up.
- 🎟️ **Member rates, trips and partner gym access** surfaced without menu digging.

**[🌐 joyizm.com](https://joyizm.com)** · **[App Store](https://apps.apple.com/us/app/joyizm/id1591948916)** · **[Google Play](https://play.google.com/store/apps/details?id=com.rezy360.joyizm)**

---

## 04 · Selected repositories

### 🏢 e-biz-3.0 — enterprise app platform

HRMS, CRM, travel and hotel modules with live location tracking in one mobile app, shipped in versioned releases with a running changelog.

`Dart` · `Flutter` · [View repo →](https://github.com/EswarVarma91/e-biz-3.0)

### 🫁 ventilator — medical device app

Flutter app built with Zyna MedTech for a Covid-19 ventilator product.

`Dart` · `Flutter` · [View repo →](https://github.com/EswarVarma91/ventilator)

### 🧪 flutter_training — practice project

Scratch space for Flutter experiments and UI exercises.

[View repo →](https://github.com/EswarVarma91/flutter_training)

**[All repositories →](https://github.com/EswarVarma91?tab=repositories)**

---

## 05 · How a screen gets shipped

```mermaid
flowchart TD
    A[Design handoff] --> B[Tokens and shared components]
    B --> C[Screen build]
    C --> D[Empty, loading and error states]
    D --> E[Accessibility and responsive pass]
    E --> F[Ship and measure]
```

> [!TIP]
> **My rule of thumb:** if a second screen needs the same block, it becomes a component before it gets built twice. Design debt compounds faster than technical debt.

---

## 06 · Contact

|  |  |
|:--|:--|
| 📧 **Email** | [varmapanumetcha02@gmail.com](mailto:varmapanumetcha02@gmail.com) |
| 📱 **Phone / WhatsApp** | [+91 9014832822](tel:+919014832822) · [Message on WhatsApp](https://wa.me/919014832822) |
| 💻 **GitHub** | [@EswarVarma91](https://github.com/EswarVarma91) |

<!-- Add your LinkedIn and it goes straight into the badge row above:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/YOUR-HANDLE)

and as a row in the contact table:

| 💼 **LinkedIn** | [your-name](https://www.linkedin.com/in/YOUR-HANDLE) |

-->

**Open to conversations about frontend architecture, design systems and mobile UI.**

---

<details>
<summary><b>🛠️ Full stack</b> — tap to expand</summary>

<br>

**Core**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)

**Mobile & cross-platform**

![Ionic](https://img.shields.io/badge/Ionic-3880FF?style=flat-square&logo=ionic&logoColor=white)
![Capacitor](https://img.shields.io/badge/Capacitor-119EFF?style=flat-square&logo=capacitor&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)

**Styling & tooling**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

</details>

<details>
<summary><b>📊 GitHub in numbers</b> — tap to expand</summary>

<br>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=EswarVarma91&show_icons=true&hide_border=true&title_color=6C63FF&icon_color=00C2A8&text_color=808080&bg_color=00000000" alt="GitHub stats" width="440" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=EswarVarma91&layout=compact&hide_border=true&title_color=6C63FF&text_color=808080&bg_color=00000000&langs_count=8" alt="Top languages" width="380" />

<img src="https://streak-stats.demolab.com/?user=EswarVarma91&hide_border=true&stroke=6C63FF&ring=00C2A8&fire=FF6B6B&currStreakLabel=6C63FF" alt="GitHub streak" width="440" />

![Profile views](https://komarev.com/ghpvc/?username=EswarVarma91&style=flat-square&color=00C2A8&label=profile+views)

</div>

</details>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=00C2A8&height=90&section=footer">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=9FF3E8&height=90&section=footer" alt="" width="100%">
</picture>
