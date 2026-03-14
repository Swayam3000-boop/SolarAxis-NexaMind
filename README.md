# ☀️ SolarAxis — Intelligent Solar Energy Platform

A full-featured solar energy monitoring and net-metering app for prosumers and grid operators.

## 🚀 Deploy to GitHub Pages

1. Upload all files to a GitHub repo
2. Go to **Settings → Pages → Source**: `main` branch, `/ (root)`
3. Live at `https://<username>.github.io/<repo>/`

No build step needed — pure static HTML/CSS/JS.

## 🔑 Demo Credentials

### Prosumer Login
| Email | Password |
|-------|----------|
| `demo@solaraxis.com` | `demo1234` |
| `admin@solaraxis.com` | `admin123` |
| `installer@solaraxis.com` | `install1` |

### Grid Operator Login
| Operator ID | Access Key |
|-------------|------------|
| `cesc@discom.gov.in` | `grid2024` |
| `msedcl@discom.gov.in` | `grid2024` |
| `bescom@discom.gov.in` | `grid2024` |

## 📁 Structure

```
solaraxis/
├── index.html                 ← Full app
├── manifest.json              ← PWA manifest
├── 404.html
├── .nojekyll
├── .gitignore
├── README.md
└── assets/
    ├── icons/favicon.svg
    └── data/dashboard_data.json
```

## 🛠 Local Development

```bash
npx serve .
# or
python3 -m http.server 8080
```
