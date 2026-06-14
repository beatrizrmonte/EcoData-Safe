# ♻️ EcoData Safe: Secure Electronic Disposal Platform

> A web and mobile platform specialized in secure data sanitization and sustainable disposal of electronic devices.
Developed as a Capstone Project (*Projeto Integrador*) for the **Systems Analysis and Development Program** at **Senac College**.

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Senac](https://img.shields.io/badge/Institution-Senac%20College-blue)](https://www.senac.br/)
[![LGPD](https://img.shields.io/badge/Compliance-LGPD%20Ready-blueviolet)](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm)

---

## 📋 Project Overview

**EcoData Safe** bridges the gap between digital security and environmental sustainability. The platform addresses a critical dual challenge: protecting users' privacy when parting with old hardware and ensuring electronic waste (e-waste) is recycled according to strict environmental guidelines.

Through our platform, users can request verified data wiping, backups, and sustainable hardware disposal, receiving a legally binding certificate at the end of the life cycle.

### Key Service Modalities

* **Total Disposal (*Descarte Total*):** For non-reusable hardware. Includes certified data overwriting, physical device destruction, and eco-friendly components recycling.
* **Backup & Wipe:** Safely archives photos, contacts, and documents to an encrypted cloud drive before executing absolute data and hardware destruction.
* **Technical Cleaning (*Limpeza Técnica*):** Tailored for users looking to sell or donate working devices. Executes deep data sanitization (wipe) and resets the hardware to factory settings, returning a clean device with a safety certificate.

---

## 🔒 LGPD & Data Privacy Compliance (Lei Geral de Proteção de Dados)

Because this application processes deeply personal and sensitive user data through backup storage and absolute device sanitization, privacy by design is a core architecture requirement in full compliance with Brazilian Federal Law nº 13.709/2018 (LGPD).

### Implemented Privacy & Quality Standards:

* **Legal Basis & Explicit Consent (Art. 7º & 11):** Data handling and physical destruction workflows are only initiated upon explicit formal user authorization recorded in the platform.
* **Irreversible Sanitization:** The core data erasure service implements deep overwriting techniques, ensuring that once a permanent wipe is confirmed, data recovery is mathematically impossible (supporting the *Direito ao Esquecimento*).
* **End-to-End Cryptography:** All data packages transferred during cloud backups or tracking updates are encrypted in transit and at rest.
* **Legal Accountability:** Upon completion of any cycle, the platform generates a cryptographically signed Digital Certificate containing execution timestamps, hardware IDs, and the specific erasure method applied.

---

## 🛠️ Tech Stack & Management

* **Design & Prototyping:** Figma, Canva
* **AI-Assisted Development:** Lovable
* **Core Documentation & Flow:** Microsoft Word, Outlook Shared Environment
* **Primary Communication Hub:** WhatsApp & Synchronous Agile Meetings

---

## ⚙️ Getting Started (Local Development)

Follow these steps to set up the project environment locally.

### 1. Prerequisites

Ensure you have installed:
* [Git](https://git-scm.com)
* [Node.js](https://nodejs.org/) (v18.0.0 or higher)
* A modern web browser or mobile emulator

### 2. Configuration (`.env`)

Create a `.env` file in your server directory to manage cryptographic tokens and system parameters:

<code>
PORT=3000
DATABASE_URL="mysql://user:password@localhost:3306/ecodatasafe_db"
JWT_SECRET="secure_system_token_string_here"
</code>

### 3. Setup and Execution

<code>
# 1. Clone the repository
git clone https://github.com/your-username/ecodata-safe.git
cd ecodata-safe

# 2. Install dependencies
npm install

# 3. Run Development Environment
npm run dev
</code>

---

## 📊 Core API Endpoints (Privacy & Tracking Architecture)

| Method | Endpoint | Description | LGPD / Scope Relevance |
| :--- | :--- | :--- | :--- |
| **POST** | `/api/services/request` | Registers a new disposal/wipe request with hardware specs | Formal user consent captured |
| **GET** | `/api/tracking/:id` | Real-time tracking of hardware stages with validated timestamps | Transparency & Accountability |
| **POST** | `/api/backup/upload` | Streams encrypted data into secure temporary cloud drives | Cryptographic security by design |
| **GET** | `/api/certificates/:id/download` | Downloads the legally valid digital Certificate of Destruction | Legal compliance and audit trail |

---

## 📝 Future Improvements (What We'd Do Next)

If we had another semester to expand the technical scope, we plan to implement:
* **Industrial API Integrations:** Build automated webhook connectors with third-party recycling hubs (like *Reeecicle*) to feed live shipping logistics directly into our tracking module.
* **Automated Device Handshake:** Develop a lightweight client-side script to auto-detect hardware specifications (IMEI, Brand, Storage) when connected via USB, minimizing manual user input errors.
* **Ephemeral Cloud Optimization:** Implement automated cron jobs to purge backup servers immediately after user confirmation, minimizing data holding risks.

---

## 👥 Authors & Project Team

* **Beatriz Ramos do Monte** - Project Manager & Schedule Controller
* **Ana Alice Rodrigues dos Santos** - Requirements Analyst
* **Isael da Silva Souza** - Core Developer (Phase 1 Execution)
* **Estevão Ferreira de Farias** - Core Developer (Phase 1 Execution)
* **Benjamim Muniz da Silva** - Quality Assurance & Testing Engineer
* **Academic Advisor / Professor**: Prof. Samantha Pimentel

* **Tech English Course Professor**: Prof. Leonardo Trevas

---

### 📂 References & Methodological Support

This project planning and documentation structure was developed based on the guidelines and frameworks provided in the following institutional files:
* `modelos de roteiro de gestao de projetos (1).pdf`
* `mockup readme ads.docx`
