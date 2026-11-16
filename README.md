# Mohamed Emad (Mohamed Harf)

<div align="center">

```
  ____        _   _                   ____             _                  _ 
 |  _ \ _   _| |_| |__   ___  _ __   | __ )  __ _  ___| | _____ _ __   __| |
 | |_) | | | | __| '_ \ / _ \| '_ \  |  _ \ / _` |/ __| |/ / _ \ '_ \ / _` |
 |  __/| |_| | |_| | | | (_) | | | | | |_) | (_| | (__|   <  __/ | | | (_| |
 |_|    \__, |\__|_| |_|\___/|_| |_| |____/ \__,_|\___|_|\_\___|_| |_|\__,_|
        |___/                                                                
```

### **Senior Python & Django Backend Engineer | System Architecture & Automation Specialist**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohamed-harf-3218)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:Mohamedharf@gmail.com)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/mohamedharf)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/share/14ukUnxASnF/)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201070488898)

---

</div>

## 📌 Executive Summary

I specialize in engineering production-ready, fault-tolerant enterprise backends, high-concurrency commerce engines, and autonomous data extraction pipelines. With deep expertise across the **Python**, **Django**, and **FastAPI** ecosystems, I design systems that balance robust domain business logic with high-throughput asynchronous execution, strictly modeled relational schemas, and hardened security.

- 🏗️ **Enterprise Architecture**: Multi-tenant ERP/CRM engines, double-entry financial ledgers, multi-party settlement systems, and wholesale/retail fulfillment workflows.
- ⚡ **High-Scale Pipelines & Automation**: Distributed web scraping infrastructure, anti-bot mitigation (undetected browser automation & fingerprint rotation), and Arabic OCR document pipelines with Celery and Redis.
- 🛡️ **Production Reliability**: Containerized deployments with Docker, Linux system tuning, test-driven validation, and automated CI/CD delivery.

---

## ⚡ Executive Engineering Scope & Impact

```text
┌──────────────────────────────────────────────┬──────────────────────────────────────────────┐
│ ⚡ EXTRACTION & PIPELINE THROUGHPUT          │ 🛡️ FINANCIAL INTEGRITY & LEDGER CONSISTENCY │
│  • 70% runtime reduction via smart dedupe    │  • 100% ACID double-entry accounting ledgers │
│  • Evasive bot-detection bypass & rotation   │  • Cryptographic POS balance debit & FIFO    │
│  • Multi-engine fallback & auto-recovery     │  • Zero-drift multi-party settlements        │
├──────────────────────────────────────────────┼──────────────────────────────────────────────┤
│ 🧠 AUTONOMOUS AGENTS & ASYNC ORCHESTRATION   │ 🌐 LOCALIZATION & DEVELOPER EXPERIENCE (DX)  │
│  • 7 decoupled lifecycle autonomous agents   │  • Native bi-directional RTL/LTR & Arabic    │
│  • Distributed Celery task pools & Redis     │  • Full OpenAPI / Swagger interactive specs  │
│  • Isolated sandboxed execution environments │  • Single-command Dockerized staging & CI/CD │
└──────────────────────────────────────────────┴──────────────────────────────────────────────┘
```

---

## 🧠 Engineering Philosophy & Architectural Principles

I approach software engineering with a staff-level focus on operational predictability, long-term maintainability, and domain isolation:

1. **ACID Integrity over Speed in Financial & Core Domains:**
   Money, inventory, and legal contracts demand absolute consistency. I enforce row-level locking (`select_for_update()`), atomic transactions, and strict database-level constraints before optimizing throughput.

2. **Decoupled Asynchrony by Default:**
   User-facing request-response cycles must remain sub-second. Any process requiring more than 200ms—such as browser scraping, optical character recognition (OCR), audio transcription, and payment reconciliation—is strictly offloaded to distributed **Celery** workers backed by **Redis**.

3. **Stealth & Evasion by Design:**
   Modern web data pipelines cannot rely on naive HTTP requests. I engineer automated scrapers with browser fingerprint rotation, stealth CDP flags, and intelligent search-engine fallback mechanisms to guarantee 99.9% ingestion reliability without IP bans.

4. **Strict Domain Boundary & Information Masking:**
   Business secrets (such as factory manufacturing costs in wholesale platforms or internal merchant markups) are never sanitized at the presentation layer alone. Masking is enforced deeply within service layer managers and ORM querysets to ensure zero data leakage across APIs.

5. **Developer Ergonomics & API-First Contracts:**
   Every backend is built to empower frontend engineers and integrators. All APIs adhere to clean REST principles, typed request schemas, and comprehensive **OpenAPI/Swagger** documentation.

---

## 🏛️ System Architecture Topology

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                       CLIENT & INTEGRATION TOUCHPOINTS                      │
│     [ Web & React PWAs ]      [ Mobile Clients ]      [ POS Terminals ]     │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │ HTTPS / WSS / REST
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│                           EDGE & SECURITY GATEWAY                           │
│     [ Nginx Reverse Proxy ] ──► [ Rate Limiting & SSL ] ──► [ RBAC Guard ]   │
└──────────────────────────────────────┬──────────────────────────────────────┘
                                       │
                                       ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│                           CORE APPLICATION ENGINE                           │
│                     [ Django 5 / 6 ]  &  [ FastAPI ]                        │
│                                                                             │
│   • Domain Business Logic               • Double-Entry Financial Ledger     │
│   • Tiered Pricing & Margin Engine      • Role-Based Access Control (RBAC)  │
│   • Payment Webhooks (Paymob HMAC)      • RESTful API Serialization         │
└───────────────────────┬─────────────────────────────┬───────────────────────┘
                        │ Synchronous                 │ Asynchronous Events
                        ▼                             ▼
┌───────────────────────────────────┐   ┌─────────────────────────────────────┐
│       PERSISTENCE & CACHE         │   │   DISTRIBUTED TASK ORCHESTRATION    │
│ • PostgreSQL 16 (ACID Relational) │   │ • Redis (Message Broker & Cache)    │
│ • Database Connection Pooling     │   │ • Celery Worker Pools & Beat        │
└───────────────────────────────────┘   └──────────────────┬──────────────────┘
                                                           │
                                                           ▼
┌─────────────────────────────────────────────────────────────────────────────┐
│                    HIGH-SCALE AUTOMATION & AI WORKERS                       │
│  • Playwright / Selenium-Stealth Ingestion Pipelines                        │
│  • Tesseract Arabic OCR Document Extraction Engines                         │
│  • Local Speech-to-Text Transcription via Faster-Whisper                    │
│  • Multi-Agent Autonomous Orchestration & Scouting                          │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 🚀 Public Engineering Portfolio & Flagship Systems

### 1. Enterprise FinTech, HealthTech & ERP/CRM Platforms

| Project | System Architecture & Core Capabilities | Tech Stack |
| :--- | :--- | :--- |
| [**Phyzioline**](https://github.com/mohamedharf/phyzioline-healthtech-platform)<br>`phyzioline-healthtech-platform` | **Next-Gen Enterprise Telehealth, Clinical EHR, Medical LMS & Financial Ledger CRM**.<br>• Unifies clinical physiotherapy, electronic health records (EHR), telemedicine consultations, and medical e-commerce.<br>• Features a mission-critical **double-entry financial ledger engine** and comprehensive multi-role CRM suite.<br>• High-concurrency asynchronous task handling, OpenAPI/Swagger API documentation, and Docker orchestration. | `Python 3.12+` `Django 5.2` `PostgreSQL 16` `Celery 5.5` `Redis` `Docker` `Swagger` |
| [**Vaetcher**](https://github.com/mohamedharf/vaetcher)<br>`vaetcher` | **Enterprise Medical Hospitality Voucher & Multi-Party Settlement Engine**.<br>• Real-time cryptographic balance debiting at Point-of-Sale (POS) registers eliminating paper vouchers.<br>• **Multi-Voucher FIFO Waterfall Deduction Engine** & dynamic merchant markup network.<br>• Automated **Triple-Tier Financial Settlements** across pharma sponsors, hospitality venues, sales reps, and physicians.<br>• Vector CR80 digital pass generation and bi-directional Arabic PDF reporting engine. | `Python 3.11+` `Django 5.2` `Django Unfold` `Tailwind CSS` `i18n RTL/LTR` `ACID Audited` |
| [**GMaps Lead CRM**](https://github.com/mohamedharf/-gmaps-lead-crm)<br>`-gmaps-lead-crm` | **End-to-End B2B Lead Generation, Async Email Enrichment & Sales CRM**.<br>• Automated lead extraction from Google Maps with anti-detection browser automation.<br>• Asynchronous corporate email hunting & enrichment pipeline with live log feeds.<br>• Tiered sales team distribution, multi-level commission tracking, and **Paymob online payment integration**. | `Python 3.12` `Django 6.0` `Selenium Stealth` `Tailwind CSS` `Bootstrap 5.3` `Paymob HMAC` |
| [**MEN EL-MASNA3**](https://github.com/mohamedharf/men-elmasna3)<br>`men-elmasna3` *(Enterprise)* | **Direct-to-Factory Hybrid B2C & B2B Knitwear E-Commerce & Fulfillment Platform**.<br>• Dynamic tiered wholesale pricing with minimum thresholds and merchant deposit validation.<br>• Strict factory isolation: sanitizes factory costs/identities from public and merchant APIs.<br>• Dual logistics engine (retail flat-rate vs. weight-calibrated wholesale across 27 governorates) and Saturday batch fulfillment. | `Python` `Django 5.1` `DRF` `React 18` `Vite` `PostgreSQL` `Tailwind CSS` `GitHub Actions` |

### 2. Autonomous AI Agents & Intelligent Automation

| Project | System Architecture & Core Capabilities | Tech Stack |
| :--- | :--- | :--- |
| [**FreelanceOS**](https://github.com/mohamedharf/FreelanceOS)<br>`FreelanceOS` | **Autonomous AI Freelance Agency & Deal Lifecycle Operating System (v4.0)**.<br>• Coordinates **7 specialized autonomous agents** (Lead Scout, Intelligence Profiler, Solution Architect, Proposal Strategist, Deal Room Negotiator, Workspace Orchestrator, Evolution Engine).<br>• Headless multi-platform scouting across 6 international platforms, client psychometrics, interactive deal rooms, and sandboxed Git workspaces. | `Python 3.10+` `Django 5` `DRF` `React 18` `Playwright` `Celery` `Redis` `Tailwind CSS` |
| [**TubePulse AI**](https://github.com/mohamedharf/tubepulse-ai)<br>`tubepulse-ai` | **YouTube Channel Intelligence, Algorithmic SEO & Stealth Studio Automation Engine**.<br>• Bridges algorithmic SEO evaluation with undetectable browser automation (`undetected-chromedriver`).<br>• Automated YouTube Studio management, metadata optimization, competitor gap heuristics, and task scheduling.<br>• Dockerized deployment with 100% test coverage across core extraction and execution modules. | `Python 3.11+` `Django 5.1` `Selenium 4.20+` `Undetected-ChromeDriver` `Docker` `GitHub Actions` |
| [**Maraya**](https://github.com/mohamedharf/mirror-mind-)<br>`mirror-mind-` | **Behavioral Reflection Engine & Privacy-Centric Personal Intelligence Platform**.<br>• Mirrored human behavioral analysis through asynchronous cognitive ingestion and multi-horizon analytics.<br>• On-device local speech-to-text synthesis via **Faster-Whisper (CTranslate2)**.<br>• Decoupled Celery worker pools, Redis caching, and offline-capable React PWA frontend. | `Python` `Django` `React PWA` `Faster-Whisper` `Celery` `Redis` `OAuth2` |

### 3. Data Engineering, High-Scale Scraping & OCR Pipelines

| Project | System Architecture & Core Capabilities | Tech Stack |
| :--- | :--- | :--- |
| [**TenderPulse**](https://github.com/mohamedharf/monaqasat-core)<br>`monaqasat-core` | **Government Procurement Intelligence Platform & Arabic OCR Pipeline**.<br>• Dual-engine scraping: Playwright headless browser for dynamic portals + Google Dorking archive fallback.<br>• Arabic OCR pipeline converting RFP PDFs into high-res images and indexing text with **Tesseract OCR**.<br>• Real-time dark-mode operational dashboard with live terminal stream and RESTful Excel/CSV export. | `Python` `Django` `DRF` `Playwright` `Tesseract OCR` `Celery` `Redis` `Docker` `PostgreSQL` |
| [**Perenual Plant Scraper**](https://github.com/mohamedharf/scrap_plan)<br>`scrap_plan` | **Botanical Species Extraction Engine & Searchable Catalog**.<br>• Headless Selenium automation handling infinite-scroll pagination paired with BeautifulSoup4 parsing.<br>• Browser-based control dashboard with start/stop toggles, auto-polling log stream, and multi-field deduplication.<br>• Automated local image archiving and full-text faceted botanical catalog. | `Python` `Django` `Selenium` `BeautifulSoup4` `SQLite` `Bootstrap` `Requests` |

---

## 🛠️ Technical Stack & Tooling

### **Backend & Frameworks**
![Python](https://img.shields.io/badge/Python_3-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/Django_REST_Framework-A30000?style=for-the-badge&logo=django&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

### **Databases & Async Orchestration**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white)

### **DevOps, Infrastructure & OS**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Ubuntu Linux](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

### **Automation, Scraping & AI**
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white)
![BeautifulSoup4](https://img.shields.io/badge/BeautifulSoup4-59666C?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)

---

## 📊 Repository Languages Distribution

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=mohamedharf&theme=tokyonight" alt="Top Languages by Repo" width="55%" />

</div>

---

## 📬 Connect & Direct Inquiries

I welcome discussions regarding senior backend engineering roles, enterprise architecture consultations, high-scale scraping infrastructure, and custom ERP/CRM platforms.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohamed-harf-3218)
[![Email](https://img.shields.io/badge/Email-Direct_Message-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:Mohamedharf@gmail.com)
[![Telegram](https://img.shields.io/badge/Telegram-Message-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/mohamedharf)
[![Facebook](https://img.shields.io/badge/Facebook-Profile-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/share/14ukUnxASnF/)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Chat-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201070488898)

</div>

<br>

| Channel | Direct Identifier / Link |
| :--- | :--- |
| **Email** | [`Mohamedharf@gmail.com`](mailto:Mohamedharf@gmail.com) |
| **LinkedIn** | [`linkedin.com/in/mohamed-harf-3218`](https://www.linkedin.com/in/mohamed-harf-3218) |
| **Telegram** | [`@mohamedharf`](https://t.me/mohamedharf) |
| **WhatsApp** | [`+20 107 048 8898`](https://wa.me/201070488898) |
| **Facebook** | [`facebook.com/share/14ukUnxASnF/`](https://www.facebook.com/share/14ukUnxASnF/) |
