# AirGuard — AI-Powered Carbon Monitoring Platform

> Research portfolio and AI app prototypes from the **Asian Hackathon for Green Future 2026** at VinUniversity, Ho Chi Minh City, Vietnam.

[![Event](https://img.shields.io/badge/Event-Asian%20Hackathon%20for%20Green%20Future%202026-coral?style=flat-square&labelColor=gold)]()
[![Team](https://img.shields.io/badge/Team-AirGuardian-blue?style=flat-square)](#)
[![Platform](https://img.shields.io/badge/Platform-iOS%20%2B%20Research-blue?style=flat-square)](#)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)](#)

---

## Overview

**AirGuard** is a privacy-first mobile app concept that calculates CO2 emissions from urban transport — entirely on-device, with no backend, no cloud, and no data leaving the phone.

Built during the **Asian Hackathon for Green Future 2026** at **VinUniversity**, this repository contains:
- Research on CO2 emission factors for vehicles in Vietnam
- A portfolio of 7 AI-powered carbon tracking app ideas
- Live interactive prototypes (CarbonMind chat, FoodPrint calculator, CarbonHive gamification)

---

## Project Structure

```
airguard-vinuni-hackathon/
├── dataset_research.html     ← Full technical research (~103 KB)
│   ├── Emission factor database (13 vehicle types)
│   ├── DEFRA 2025 / ICCT / IPCC / ADB / GHG Protocol comparisons
│   ├── Carbon equivalents (Taiwan EPA CFP Database)
│   ├── Vietnam/HCMC context (9M motorbikes, 800K cars)
│   └── AirGuard app specification
├── carbon-portfolio.html     ← AI app portfolio (~88 KB)
│   ├── 7 ranked AI app ideas with comparison table
│   ├── Live prototypes (CarbonMind, FoodPrint, CarbonHive)
│   └── Recommended roadmap
└── README.md                 ← This file
```

---

## Highlights

### 7 AI App Ideas Explored

| Rank | App | Domain | Status |
|------|-----|--------|--------|
| 1 | **CarbonMind** | AI conversational coach | ⭐ Recommended |
| 2 | **FoodPrint** | AI meal photo tracker | Runner Up |
| 3 | **CarbonHive** | Gamified community challenges | Third Place |
| 4 | **TransitIQ** | Passive commute ML analyzer | Strong |
| 5 | **FootprintSync** | Bank transaction auto-tracker | Vision |
| 6 | **SupplyChain Lens** | Product barcode scanner | Experimental |
| 7 | **GridPulse** | Smart home carbon optimizer | Strong |

### Emission Factors — Key Data

| Vehicle Type | Factor (kg CO2/veh-km) | Source |
|-------------|----------------------|--------|
| Motorbike (petrol) | 0.085 | ICCT Asia 2024 |
| Car small (petrol) | 0.1431 | DEFRA 2025 |
| Car medium (petrol) | 0.1747 | DEFRA 2025 |
| Car diesel | 0.1730 | DEFRA 2025 |
| Car hybrid | 0.1283 | DEFRA 2025 |
| Car EV | 0.000 | — |
| Bus diesel | 0.1253 | DEFRA 2025 |
| Taxi/Grab | 0.1486 | DEFRA 2025 |
| MRT / Light rail | 0.0286 | DEFRA 2025 |
| Walking | 0.000 | — |

### Data Sources

| Source | Version | Coverage |
|--------|---------|----------|
| DEFRA | 2025 | UK conversion factors (condensed set) |
| ICCT | Asia 2024 | Real-world passenger vehicle emissions |
| IPCC | 2006 / 2019 Refinement / AR6 | Tier 1 default factors |
| ADB | 2023 | Asia Sustainable Transport Outlook |
| GHG Protocol | — | Scope 3 Category 6 |
| Taiwan EPA CFP | 2024 | Carbon equivalents database |

---

## Tech Stack

```
Research       Static HTML/CSS/JS (self-contained documents)
App Concept    Expo · React Native · TypeScript
AI Features   Claude API · RAG/Vector DB
Data          DEFRA 2025 · ICCT Asia · IPCC · ADB · GHG Protocol
Compliance    ISO 14067:2018 emission factor standard
```

---

## Key App Features (AirGuard MVP)

- **3-Tap Trip Logging** — Start → Select vehicle → End
- **13 Vehicle Types** — Motorbikes, cars, buses, taxis, MRT, EVs, and more
- **Privacy by Design** — No backend, no cloud, all calculations on-device
- **Carbon Equivalents** — Makes emissions relatable (e.g., "≈ 2 cups of milk tea")
- **Daily Budget Tracker** — Based on 1.5°C science (6.8 kg CO2/day)
- **Vietnam Context** — 9M registered motorbikes, HCMC Metro Line 1 since 2024

---

## Live Prototypes

Open `carbon-portfolio.html` in a browser to interact with:

1. **CarbonMind Chat** — Type natural language ("I drove 10km by motorbike") and see CO2 calculated
2. **FoodPrint Calculator** — Select meal items and get CO2 + swap recommendations
3. **CarbonHive** — Browse community challenges, leaderboard, and earn Hive Points

---

## Getting Started

```bash
# Open research document
open dataset_research.html

# Open AI portfolio with prototypes
open carbon-portfolio.html

# Or serve locally
python3 -m http.server 8080
# → http://localhost:8080
```

---

## Awards & Recognition

- 🏆 **Asian Hackathon for Green Future 2026** — VinUniversity, May 2026
- Team: **AirGuardian** (5 members, AI & IT focus)

---

## Future Roadmap

| Version | Focus |
|---------|-------|
| MVP | On-device trip logging, 13 vehicle types, emission factors |
| V2 | Google Maps auto-distance, cross-device sync, Firebase |
| V3 | AI chat (Claude), RAG pipeline, Climatiq API integration |
| V4 | Open Banking, supply chain scanner, community features |
