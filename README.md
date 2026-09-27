# PingalaBit

**Ācārya Piṅgala's binary prosody meets modern computer science.**

A fully static, five-page interactive website built for IKS Assignment No. 6 — exploring how the *Chandaḥśāstra* (c. 3rd–2nd century BCE) laid the mathematical foundations of binary logic roughly 2,000 years before Leibniz.

🌐 **Live:** https://pingalabit.vercel.app

---

## Pages

| Page | Description |
|---|---|
| `index.html` | Landing page — hero, interactive binary demo, feature overview |
| `learn.html` | Explore & Solve — full Prastāra, Naṣṭa, Uddiṣṭa, and Meru labs with audio synthesizer |
| `quiz.html` | Timed 10-question quiz with score tracking and badge awards |
| `course.html` | Self-paced 8-module guided course with sidebar nav and progress persistence |
| `about.html` | Team roster, historical timeline, glossary, and scholarly sources |
| `404.html` | Custom branded 404 page |

---

## Tech Stack

- **Pure HTML + CSS + Vanilla JS** — zero build step, zero dependencies to install
- **Tailwind CSS** via CDN (v3 with forms + container-queries plugins)
- **Google Fonts** — Noto Serif, Inter, JetBrains Mono
- **Material Symbols Outlined** for icons
- **Web Audio API** for the metre synthesizer on the Learn page
- **localStorage** for quiz state and course progress persistence

---

## Design System

"Manuscript Brutalism" — a saffron/indigo/teal Material Design 3 palette layered over palm-leaf scanline backgrounds and manuscript-border card frames.

| Token | Value | Use |
|---|---|---|
| `primary` | `#8f4e00` | Saffron — Piṅgala, active nav, headings |
| `secondary` | `#515b90` | Indigo — Guru tiles, secondary actions |
| `tertiary` | `#006a61` | Teal — correct answers, Meru nodes |

---

## Deployment (Vercel)

This repo is pre-configured for **Vercel** via [`vercel.json`](./vercel.json).

### Deploy in 3 steps

1. Go to [vercel.com](https://vercel.com) and click **Add New → Project**
2. Import this GitHub repository (`https://github.com/Shreyas-patil07/iks`)
3. Keep default settings (Framework Preset: **Other**, Root Directory: `./`) and click **Deploy**

No build command or output directory is needed.

### What `vercel.json` configures

- **Clean URLs:** Routes `/learn`, `/quiz`, `/course`, `/about` work automatically without `.html` extension
- **Security headers:** `X-Frame-Options`, `X-Content-Type-Options`, `Referrer-Policy`, `Permissions-Policy`
- **Smart cache:** HTML pages revalidate immediately; static resources, sitemap, and robots are cached efficiently
- **Custom 404:** Automatic branded 404 error page handling

---

## Local Development

No server required — just open `index.html` directly in a browser.

For a local dev server with live reload:

```bash
# Python (built-in)
python -m http.server 8080

# Node (if installed)
npx serve .
```

Then open `http://localhost:8080`.

---

## Scholarly Sources

- Piṅgala, *Chandaḥśāstra* (c. 3rd–2nd century BCE)
- Van Nooten, B.A. (1993). "Binary numbers in Indian antiquity." *Journal of Indian Philosophy*, 21(1), 31–50.
- Halāyudha, *Mṛtasañjīvinī* commentary (10th century CE)
- Virahāṅka, *Vṛttajātisamuccaya* (c. 6th–8th century CE)
- Knuth, D.E. (2011). *The Art of Computer Programming*, Vol. 4A.

---

## Team

IKS Assignment No. 6 — Computational Prosody & Binary Mathematics  
© 2025 PingalaBit
