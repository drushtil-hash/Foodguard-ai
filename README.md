# 🥗 FOODGUARD – AI-Powered Food Waste Prevention

> **Tagline:** *Predict food waste. Redistribute food. Feed more people.*

[![Live Demo](https://img.shields.io/badge/Live%20Demo-View%20Prototype-10b981?style=for-the-badge&logo=googlechrome&logoColor=white)](https://drushtil-hash.github.io/Foodguard-ai/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-06b6d4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/drushtil-hash/Foodguard-ai)
[![AI Powered](https://img.shields.io/badge/AI-Gemini%203%20Flash-8b5cf6?style=for-the-badge&logo=google&logoColor=white)](https://deepmind.google/technologies/gemini/)
[![Hackathon](https://img.shields.io/badge/Hackathon-Project%20Submission-f59e0b?style=for-the-badge)](https://github.com/drushtil-hash/Foodguard-ai)

---

## 📌 Problem Statement

Modern food supply chains suffer from a severe structural disconnect between retail overstock and community food insecurity:

* **Inaccurate Forecasting:** Retailers and restaurants rely on static estimation tools that fail to adapt to market variables like weather shifts, local events, and changing foot traffic, resulting in massive over-ordering and spoilage.
* **Invisible Surplus:** Nearby food banks lack real-time visibility into local business overstock.
* **The 48-Hour Decay Cliff:** By the time excess food is manually identified by staff, remaining shelf life is too short for traditional recovery pipelines to safely pick up and distribute.

This creates a critical triple-bottom-line failure: severe financial shrinkage for food businesses, heavy landfill methane emissions for the environment, and persistent hunger in local communities.

---

## 💡 Solution Description

**FOODGUARD** transforms food recovery from a reactive post-spoilage effort into a proactive, predictive workflow. 

By analyzing local demand trends, satellite weather telemetry, and real-time inventory shelf-life, FOODGUARD predicts which items are at risk of expiring and automatically routes surplus food to local NGOs before it spoils.

### ⚡ Key Features

1. **Predictive Food Demand Forecasting:** Integrates point-of-sale data with live weather metrics (Open-Meteo API) to forecast footfall changes and optimize procurement orders at the source.
2. **Dynamic Expiry & Shelf-Life Monitor:** Real-time countdown tracking with automated risk status alerts (*Critical*, *Warning*, *Safe*) for all inventory batches.
3. **OpenStreetMap NGO Matcher:** Queries live geolocated community kitchens, food banks, and shelters using the OpenStreetMap Nominatim API.
4. **Predictive Pre-Expiry NGO Routing (X-Factor Feature):** Calculates exact remaining shelf-life windows and matches surplus items with optimal regional NGOs using a 4-Factor AI Engine:
   * 📍 **Distance & ETA:** Minimizes transit time to preserve freshness.
   * ❄️ **Cold-Storage Compliance:** Directs perishables exclusively to equipped facilities.
   * 📊 **NGO Capacity & Needs:** Routes food volume directly to high-need distribution centers.
   * ⏳ **Urgency Index:** Prioritizes items with the shortest remaining shelf life for priority dispatch.
5. **Logistics & Dispatch Manifests:** Generates chain-of-custody documentation and automated pick-up schedules.

---

## 🏗️ Technical Architecture
