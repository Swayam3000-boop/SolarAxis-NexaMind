# ☀️ SolarAxis — Intelligent Solar Energy Platform

A full-featured solar energy monitoring and net-metering platform for prosumers and grid operators (DISCOMs), built as a single-page progressive web app.

## 🚀 Live Demo

> Hosted on GitHub Pages: `https://<your-username>.github.io/solaraxis/`

---

## 📱 Features

### Prosumer Dashboard (SolarAxis)
- **Live generation monitoring** — real-time kW output with 2-second refresh
- **Daily export charts** — powered by real meter data (Meter 1412, NonTelecom-3P)
- **Financial analytics** — royalty earnings, monthly exports, ledger charts
- **AI Forecast** — 7-day generation forecast with actual vs predicted comparison
- **Maintenance** — panel-by-panel health scores and service records
- **Environmental Impact** — CO₂ avoided, trees equivalent, REC tracking
- **Grid & Trading** — net metering status and export rate tracking
- **SolarAI Chatbot** — Claude-powered AI assistant with real system context

### Grid Operator Portal (GridAxis)
- **Real-time prosumer inflow** dashboard
- **Locality energy heatmaps** — 6-zone view with feeder load status
- **Grid frequency & voltage** monitoring with live sparklines
- **Prosumer management** — searchable table of all registered meters
- **Financial reconciliation** — automated royalty billing and settlement ledger
- **Alerts & fault detection** — critical/warning/info event log

### Portfolio Landing Page
- Company statistics and platform overview
- Dual login entry points (Prosumer + Grid Operator)
- Mobile-responsive, scroll-animated sections

---

## 🗄️ Data

Real meter data from **Meter 1412 (NonTelecom-3P, 12 kWp, CESC Kolkata)**:
- **January 2026**: 319.9 kWh exported → ₹1,919.40 royalty (PAID)
- **February 2026**: 580.2 kWh exported → ₹3,481.20 royalty (PENDING)
- Peak day: 27 Feb 2026 at 47.6 kWh
- Anomaly: 16 Jan 2026 — negative reading (−19.2 kWh, grid absorption flagged)

The database (`assets/data/dashboard_data.json`) is auto-loaded at login.

---

## 🔑 Demo Credentials

### Prosumer Login
| Email | Password | User |
|-------|----------|------|
| `demo@solaraxis.com` | `demo1234` | Rahul Kumar — Homeowner, Kolkata |
| `admin@solaraxis.com` | `admin123` | Priya Sharma — Admin, Mumbai |
| `installer@solaraxis.com` | `install1` | Dev Nair — Installer, Bengaluru |

### Grid Operator Login
| Operator ID | Access Key | DISCOM |
|-------------|------------|--------|
| `cesc@discom.gov.in` | `grid2024` | CESC Kolkata |
| `msedcl@discom.gov.in` | `grid2024` | MSEDCL Mumbai |
| `bescom@discom.gov.in` | `grid2024` | BESCOM Bengaluru |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML5 / CSS3 / JavaScript (no framework) |
| Charts | Chart.js 4.4.1 (CDN) |
| Fonts | Syne + DM Sans (Google Fonts) |
| AI Chatbot | Anthropic Claude API (`claude-sonnet-4-6`) |
| Data | SQLite (local build) → JSON (deployed) |
| Hosting | GitHub Pages (static, single HTML file) |

---

## 📁 Project Structure

```
solaraxis/
├── index.html              # Full app (self-contained SPA)
├── manifest.json           # PWA manifest
├── README.md
├── .gitignore
├── assets/
│   ├── css/
│   │   └── app.css         # Extracted stylesheet (reference)
│   ├── js/
│   │   └── app.js          # Extracted JS logic (reference)
│   ├── data/
│   │   └── dashboard_data.json   # Real meter DB export
│   └── icons/
│       ├── favicon.svg
│       └── apple-touch-icon.svg
```

> **Note:** `index.html` is fully self-contained and works standalone. The `assets/` folder contains extracted versions for reference and future modularisation.

---

## 🌐 Deploying to GitHub Pages

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Visit `https://<username>.github.io/<repo-name>/`

No build step required — pure static files.

---

## 🔧 Local Development

```bash
# Any static server works — e.g.:
npx serve .
# or
python3 -m http.server 8080
# then open http://localhost:8080
```

---

## 📜 License

MIT — free to use, modify, and deploy.

---

*Built with SolarAxis Platform v2.0 — Anthropic Claude-powered energy intelligence.*
