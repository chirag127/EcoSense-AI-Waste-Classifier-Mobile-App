# EcoSnap-AI-Waste-Classification-Mobile-App

A state-of-the-art AI-powered mobile application designed for instant waste classification, guiding users on proper disposal methods through advanced image recognition technology.

---

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App/ci.yml?style=flat-square&logo=github)](https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App)
[![Tech Stack](https://img.shields.io/badge/Tech%20Stack-React%20Native%20%7C%20Expo%20%7C%20TypeScript-007ACC?style=flat-square&logo=react)](https://reactnative.dev/)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square&logo=creativecommons)](https://creativecommons.org/licenses/by-nc/4.0/)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App?style=flat-square&logo=github)](https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App)

---

**Star ⭐ this Repo to Support Future Development!**

---

## 🚀 Project Overview

EcoSnap is an innovative mobile application leveraging advanced AI and computer vision to help users accurately classify waste items. By simply taking a photo, users receive immediate guidance on whether an item is recyclable, compostable, or destined for landfill, complete with detailed disposal instructions. The app also maintains a history of classifications for user reference.

## 🌳 Key Features

*   **Instant Waste Classification:** Utilizes AI-powered image recognition to identify waste items in real-time.
*   **Smart Disposal Guidance:** Provides clear instructions for recycling, composting, or landfill.
*   **Comprehensive Instructions:** Offers detailed information on local disposal regulations and best practices.
*   **Classification History:** Logs past classifications for easy review and learning.
*   **User-Friendly Interface:** Designed with simplicity and ease of use in mind.

## 🏛️ Architecture

mermaid
graph TD
    A[Mobile Device (React Native/Expo)] --> B{Image Capture/Upload};
    B --> C[AI Inference Engine (On-Device/Cloud)];
    C --> D[Waste Classification API]
    D -- Item Category & Instructions --> E[User Interface];
    E --> F[History Storage (Local/Remote)];
    A -- User Interactions --> E;


## 📘 Table of Contents

*   [🚀 Project Overview](#-project-overview)
*   [🌳 Key Features](#-key-features)
*   [🏛️ Architecture](#️-architecture)
*   [📘 Table of Contents](#-table-of-contents)
*   [🤖 AI AGENT DIRECTIVES](#-ai-agent-directives)
*   [🛠️ Development Standards](#️-development-standards)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Running the App](#running-the-app)
    *   [Scripts](#scripts)
*   [📝 Contributing](#-contributing)
*   [⚖️ License](#️-license)
*   [🔒 Security](#-security)

---

## 🤖 AI AGENT DIRECTIVES

<details>
<summary>View AI Agent Directives</summary>

This repository is configured to be managed and extended by AI agents. Adherence to these directives ensures seamless integration and future compatibility.

*   **IDENTITY:** Apex Technical Authority & Elite Architect (December 2025 Edition)
*   **PRIME DIRECTIVE:** Execute with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable." Operate on December 2025 standards for 2026 readiness.
*   **OUTPUT STANDARD:** EXECUTION-ONLY results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
*   **PHILOSOPHY:** "Zero-Defect, High-Velocity, Future-Proof."

### 🧠 INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. Agents must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 💡 CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **PROJECT TYPE:** Mobile Application
*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** This project leverages **TypeScript 6.x** (Strict Mode enabled by default), **Vite 7** (with Rolldown Bundler for peak performance), **Tauri v2.x** (for native desktop capabilities if extended), and **WXT** (for future web extension development). State management adheres to **Signals** (as per the standardized approach in December 2025).
    *   **Framework:** **React Native** with **Expo** for streamlined mobile development and build processes.
    *   **Linting & Formatting:** **Biome v2** is mandated for ultra-fast, all-in-one code quality. Configuration is managed within `biome.json`.
    *   **Testing:** **Vitest** for lightning-fast unit and integration tests. **Playwright** is integrated for end-to-end testing across mobile environments.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)** principles for maintainable and scalable code structure.

### 🚀 NAMING CONVENTION
*   **Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
*   **Format:** `Title-Case-With-Hyphens`
*   **Rules:** 3 to 10 words, MUST include high-volume keywords. NO numbers, NO emojis, NO underscores, NO generic words without qualifiers. Applies to all repository and component naming.

### 🌟 CODING PRINCIPLES
*   **SOLID:** Strictly adhere to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles.
*   **DRY:** Don't Repeat Yourself. Abstract common logic and components.
*   **YAGNI:** You Ain't Gonna Need It. Build only what is necessary for current requirements.
*   **KISS:** Keep It Simple, Stupid. Favor clarity and simplicity in design and implementation.

### 🛠️ VERIFICATION COMMANDS
*   **Lint & Format:** `bun run lint:fix` (or `npm run lint:fix`)
*   **Unit Tests:** `bun run test:unit` (or `npm run test:unit`)
*   **E2E Tests:** `bun run test:e2e` (or `npm run test:e2e`)
*   **Build:** `bun run build` (or `npm run build`)

</details>

---

## 🛠️ Development Standards

### Prerequisites

*   Node.js (version 18.x or later recommended)
*   npm or Yarn (npm is used in this example)
*   Expo CLI: `npm install -g expo-cli`

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App.git
    cd EcoSnap-AI-Waste-Classification-Mobile-App
    

2.  **Install dependencies:**
    bash
    npm install
    

### Running the App

*   **Start the development server:**
    bash
    npm start
    
    or
    bash
    npx expo start
    

    This will start the Metro Bundler. You can then run the app on an iOS simulator, Android emulator, or a physical device using the Expo Go app.

### Scripts

| Script        | Description                                        |
|---------------|----------------------------------------------------|
| `start`       | Starts the Metro Bundler for development.          |
| `android`     | Builds and runs the app on an Android emulator.    |
| `ios`         | Builds and runs the app on an iOS simulator.       |
| `web`         | Builds and runs the app in a web browser.          |
| `lint`        | Runs Biome linter to check code style.
*   **Format** the code using Biome:
    bash
    npm run format
    
*   **Run Unit Tests:**
    bash
    npm run test:unit
    
*   **Run End-to-End Tests:**
    bash
    npm run test:e2e
    
*   **Build the app:**
    bash
    npm run build
    

---

## 📝 Contributing

Contributions are welcome! Please refer to the [.github/CONTRIBUTING.md](.github/CONTRIBUTING.md) file for detailed guidelines.

---

## ⚖️ License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](LICENSE) file for more details.

---

## 🔒 Security

For security-related issues, please refer to the [.github/SECURITY.md](.github/SECURITY.md) file for reporting procedures.
