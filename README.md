# 🔵 WhatsApp Blue Badge Eligibility Checker

A free, open-source tool that helps businesses and individuals determine if they qualify for the **official WhatsApp Blue Badge (Verified Business Account)** — and exactly what to do if they don't.

![WhatsApp Blue Badge Checker](https://img.shields.io/badge/WhatsApp-Blue%20Badge%20Checker-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![HTML](https://img.shields.io/badge/Built%20With-HTML%20%2F%20CSS%20%2F%20JS-orange?style=for-the-badge)

---

## 📋 What Is the WhatsApp Blue Badge?

The WhatsApp Blue Badge (also called an **Official Business Account**) is a verified checkmark ✅ that appears next to a business name in WhatsApp chats. It tells users that WhatsApp has confirmed the account belongs to a legitimate, notable business.

It is different from the standard green **WhatsApp Business Account** badge — the blue badge requires a formal application and review by Meta.

---

## ✨ Features

- ✅ **5-step guided form** — collects all relevant information without overwhelming the user
- 📊 **Smart scoring engine** — evaluates 12 weighted criteria based on WhatsApp's official policies
- 🎯 **3-tier verdict** — Highly Eligible / Partially Eligible / Not Yet Eligible
- 🔍 **Per-criteria breakdown** — each requirement shown as Pass ✓ / Warning ⚠️ / Fail ✗ with specific advice
- 🚨 **6 violation/issue scenarios** with step-by-step resolution guides:
  - Badge approved but not visible in the app
  - Account flagged for spam or mass messaging
  - Policy violation or account ban
  - Impersonation or identity dispute
  - Application previously rejected
  - No issues — just checking eligibility
- 📱 **Fully responsive** — works on mobile, tablet, and desktop
- ⚡ **Zero dependencies** — pure HTML, CSS, and JavaScript; no frameworks, no build tools
- 🌐 **Works offline** — everything runs client-side; no data is sent to any server

---

## 🚀 Live Demo

> You can host this on [GitHub Pages](https://pages.github.com/) for free — see the [Deployment](#-deployment) section below.

---

## 📁 Project Structure

```
whatsapp-badge-checker/
│
├── index.html          # Main application (single-file)
├── README.md           # This file
├── LICENSE             # MIT License
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Pages auto-deploy (optional)
```

> The entire app lives in a single `index.html` — no build step, no dependencies, no configuration required.

---

## 🛠️ Local Setup

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/whatsapp-badge-checker.git

# 2. Navigate into the folder
cd whatsapp-badge-checker

# 3. Open in your browser
open index.html
# or on Linux:
xdg-open index.html
# or on Windows:
start index.html
```

That's it — no `npm install`, no build step. Just open `index.html` in any modern browser.

---

## 🌐 Deployment

### Option 1 — GitHub Pages (Recommended, Free)

1. Fork or clone this repository
2. Go to your repo → **Settings** → **Pages**
3. Under **Source**, select `main` branch and `/ (root)`
4. Click **Save**
5. Your site will be live at: `https://YOUR_USERNAME.github.io/whatsapp-badge-checker/`

### Option 2 — Netlify (Drag & Drop)

1. Go to [netlify.com](https://netlify.com) and sign up
2. Drag and drop the project folder into the Netlify dashboard
3. Your site is live instantly with a free subdomain

### Option 3 — Vercel

```bash
npm i -g vercel
vercel --prod
```

### Option 4 — Any Static Host

Since the app is a single HTML file, it can be deployed on:
- Amazon S3 + CloudFront
- Cloudflare Pages
- Firebase Hosting
- Any shared web hosting (cPanel, etc.)

---

## 📊 How the Scoring Works

The eligibility score (0–100%) is calculated across **12 weighted criteria**:

| Criterion | Max Points | Why It Matters |
|-----------|-----------|----------------|
| WhatsApp Account Type (API vs App) | 20 | Blue Badge requires the WhatsApp Business API |
| Meta Business Manager Connected | 10 | Required for badge application |
| Business Profile Completeness | 10 | All 8 fields must be filled |
| Legal Business Registration | 10 | Authenticity requirement |
| Official Website | 8 | Proves business legitimacy |
| Facebook Page + Verification | 8 | Strongly linked to Meta's review process |
| Social Media Presence (platforms) | 10 | Notability signal |
| Social Following Size | 8 | Demonstrates brand reach |
| Media / Press Coverage | 10 | Key notability factor |
| Notability Signals (Wikipedia etc.) | 6 | Additional recognition proof |
| Business Age | 5 | Stability and authenticity |
| Google Business Presence | 5 | Online credibility |

**Verdict thresholds:**
- **75–100%** → Highly Eligible — Ready to apply
- **50–74%** → Partially Eligible — Address gaps first
- **0–49%** → Not Yet Eligible — Requirements to complete

---

## 📜 WhatsApp Blue Badge Eligibility Requirements (Summary)

Based on Meta's official documentation, a business must be:

1. **Authentic** — a real, legally registered business entity
2. **Using WhatsApp Business API** — not just the free app
3. **Connected to Meta Business Manager** — verified account ownership
4. **Notable** — recognized by media, widely searched, or well-known in its industry
5. **Policy-compliant** — no active violations or bans

> The Blue Badge is **not purchasable** — it cannot be bought with an ad spend or Meta subscription. It is granted exclusively through Meta's review process.

---

## 🚨 Issue-Specific Guides Included

| Scenario | Resolution Steps Provided |
|----------|--------------------------|
| Badge approved but not visible | Cache fix, API display issue, Meta support contact |
| Account flagged for spam | Quality rating recovery, opt-in compliance, messaging best practices |
| Policy violation / ban | Appeal process, violation identification, compliance steps |
| Impersonation / identity issue | Report process, Meta IP form, customer alert steps |
| Application rejected | Wait period, common rejection reasons, reapplication checklist |

---

## 🤝 Contributing

Contributions are welcome! Here's how:

```bash
# Fork the repo, then:
git checkout -b feature/your-improvement
# Make your changes to index.html
git commit -m "feat: describe your change"
git push origin feature/your-improvement
# Open a Pull Request
```

**Ideas for contributions:**
- Add more languages / translations
- Add a PDF export of the eligibility report
- Add dark mode toggle
- Improve scoring algorithm based on new Meta policies
- Add more violation types

---

## 🐛 Reporting Issues

Found a bug or have a suggestion? [Open an issue](../../issues/new) with:
- What you expected to happen
- What actually happened
- Browser and OS you're using

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Disclaimer

This tool is an independent eligibility assessment aid based on publicly available WhatsApp and Meta policies. It is **not affiliated with, endorsed by, or connected to Meta, WhatsApp, or any of their subsidiaries**. Eligibility scores are estimates only — final approval decisions are made solely by Meta's review team. Policies may change; always check [business.whatsapp.com](https://business.whatsapp.com) for the most up-to-date requirements.

---

## 🙏 Acknowledgements

- [WhatsApp Business Platform Documentation](https://developers.facebook.com/docs/whatsapp)
- [Meta Business Help Center](https://business.facebook.com/help)
- [Google Fonts — Syne & DM Sans](https://fonts.google.com)

---

<p align="center">Made with ❤️ to help businesses get verified on WhatsApp</p>
