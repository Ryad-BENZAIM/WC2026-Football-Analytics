# ⚽ WC2026 Football Analytics — Pre-Tournament Report

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi&logoColor=black)
![pandas](https://img.shields.io/badge/pandas-2.0-150458?logo=pandas&logoColor=white)
![WC2026](https://img.shields.io/badge/FIFA-World%20Cup%202026-red)
![Status](https://img.shields.io/badge/Status-Published-brightgreen)

> **Pre-tournament data analysis of Algeria 🇩🇿 and Saudi Arabia 🇸🇦 — World Cup 2026**  
> Built with Python · Power BI · Published on LinkedIn

---

## 📌 Project Overview

This project is a **portfolio data analytics project** combining football domain expertise with data engineering and visualization skills.

The objective: build a credible, data-driven pre-tournament report on two World Cup 2026 teams — Algeria (Group D) and Saudi Arabia (Group H) — targeting the Saudi Arabia and Algeria football analytics community on LinkedIn.

**What makes this project different:**
- Data collected from verified sources (FotMob, ESPN, BeSoccer, Transfermarkt)
- Methodological transparency (Arab Cup squad limitations documented, outliers flagged)
- Full pipeline: Python → CSV → Power BI → LinkedIn carousel

---

## 📊 Dashboard Preview

### Algeria 🇩🇿
![Algeria Dashboard](screenshots/dashboard_algeria.png)

### Saudi Arabia 🇸🇦
![Saudi Arabia Dashboard](screenshots/dashboard_ksa.png)

---

## 🗂️ Repository Structure

```
WC2026-Football-Analytics/
│
├── data/
│   ├── WC2026_all_games.csv          # 15 matches (5 DZA + 10 KSA)
│   ├── WC2026_stats_overview.csv     # KPI summary — squad complet only
│   ├── WC2026_stats_ksa_periods.csv  # Arab Cup vs Full Squad comparison
│   ├── WC2026_groups.csv             # Group stage opponents + FIFA ranking
│   ├── WC2026_players_full.csv       # 10 key players (DZA + KSA)
│   ├── WC2026_players_algeria.csv    # 5 Algeria players
│   └── WC2026_players_ksa.csv        # 5 Saudi Arabia players
│
├── carousels/
│   ├── carousel_algerie_cdm2026_EN.pptx   # 12-slide LinkedIn carousel
│   └── carousel_ksa_cdm2026_EN.pptx       # 11-slide LinkedIn carousel
│
├── screenshots/
│   ├── dashboard_algeria.png
│   └── dashboard_ksa.png
│
├── rebuild_csvs.py    # Main Python script — data construction + export
└── README.md
```

---

## 🇩🇿 Algeria — Key Data

| Metric | Value |
|--------|-------|
| Last 5 matches (Full Squad) | 3W · 1D · 1L |
| Points / 15 | 10 |
| Goals Scored | 9 |
| Goals Conceded | 2 |
| Clean Sheets | 4 |
| Avg. Goals Scored | 1.8 / match |
| xG vs Nigeria (AFCON QF) | **0.13** — eliminated |

**Group D:** Argentina 🇦🇷 #3 · Austria 🇦🇹 #25 · Jordan 🇯🇴 #87

**Key Players:** Mahrez (113 caps) · Bentaleb (LOSC) · Luca Zidane (GK)  
**One to Watch:** Hadj Moussa (13G+7A Feyenoord) · Maza (Leverkusen, 20 y/o)

> ⚠️ **Methodological note:** Guatemala (FIFA #140+, 7-0) inflates offensive stats. Excluding this outlier: 2 goals in 4 competitive matches.

---

## 🇸🇦 Saudi Arabia — Key Data

| Metric | Value |
|--------|-------|
| Last 5 matches (Full Squad) | 0W · 1D · 4L |
| Points / 15 | 1 |
| Goals Scored | 2 |
| Goals Conceded | 9 |
| Clean Sheets | 1 |
| Shots on Target avg. | **1.8 / match** |

**Group H:** Spain 🇪🇸 #2 · Uruguay 🇺🇾 #16 · Cape Verde 🇨🇻 #68

**Key Players:** Salem Al-Dawsari (108 caps, 8G+8A) · Abdulhamid (RC Lens) · Al-Buraikan  
**One to Watch:** Al-Juwayr (Saudi POTS, rating 7.81) · Sultan Mandash (impact sub)

> ⚠️ **Methodological note:** Arab Cup results (2W 1D 2L) use SPL-only squad — Abdulhamid absent. Full squad stats used for all comparative analysis.  
> ⚠️ **Coach change:** Donis appointed 24/04/2026 — only 7 weeks before the tournament.

---

## 🛠️ Stack

| Tool | Usage |
|------|-------|
| **Python 3.11** | Data construction, cleaning, CSV export |
| **pandas** | DataFrame manipulation, stats calculation |
| **Power BI** | Interactive dashboard (2 pages) |
| **PowerPoint** | LinkedIn carousel (Adidas WC font) |
| **Google Colab** | Python execution environment |

---

## 📐 Methodology

**Data sources (verified):**
- Match results & stats: FotMob (Opta data), ESPN, BeSoccer
- Player stats: FotMob, Transfermarkt, SPL official
- FIFA rankings: FIFA.com (June 2026)
- Tactical analysis: Squawka, SI.com, press sources

**Data pipeline:**
```
Manual collection (FotMob/ESPN)
        ↓
Python (rebuild_csvs.py) — cleaning + structuring
        ↓
7 × CSV files
        ↓
Power BI — visualization
        ↓
LinkedIn carousel (PPTX → JPEG)
```

**Known limitations:**
- xG data unavailable for all matches (friendlies not always tracked)
- KSA Arab Cup stats excluded from main comparison (different squad composition)
- Team filtering applied manually at visual level in Power BI — relationship-based cross-filtering to be optimized in v2

---

## 📱 LinkedIn Posts

- 🇩🇿 [Algeria Pre-WC Analysis](#) ← *link to be added after publication*
- 🇸🇦 [Saudi Arabia Pre-WC Analysis](#) ← *link to be added after publication*

---

## 👤 Author

**Ryad Benzaim** — Data & AI Analyst · Riyadh 🇸🇦

- 🔗 [LinkedIn](https://www.linkedin.com/in/ryad-benzaim)
- 🐙 [GitHub](https://github.com/Ryad-BENZAIM)
- 🏟️ UEFA B License · Video Analyst · Football Operations Coordinator

> *"Football without data is just opinion."*

---

## 📄 License

Data collected from public sources for educational and portfolio purposes.  
Match statistics © respective rights holders (Opta, FotMob, ESPN).  
This project is non-commercial — portfolio use only.
