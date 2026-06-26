<h2><img src="logo.png" width="40" align="center"> Spark-Pro-Showcase</h2>

**Platform:** Android / iOS / Windows Desktop (built with Flutter)  
**Version:** 2.0.0 (Release - Production Ready)

---

## 1. Executive Summary
**Spark Pro** goes beyond traditional note-taking—it acts as a cross-platform "second brain." The application connects personal notes to an advanced AI engine (Gemini 1.5 Pro/Flash) capable of reading, comprehending, and analyzing these notes to answer any query. The app is architected with a strict focus on **Security**, **Cross-Platform Synchronization**, and **Speed**.

## 2. Technical Architecture
Built using modern technologies to ensure high performance and absolute stability across mobile and desktop:
* **Frontend:** Developed using Dart and the Flutter framework to provide a seamless, native-compiled user experience on Android and Windows.
* **Backend & Database:** Utilizes Firebase Cloud Firestore as a real-time NoSQL cloud database with offline-first persistence.
* **AI Engine:** Integrated with the Google Generative AI (Gemini API) to generate analytical text based on user data.
* **Security Layer:** Environment variable injection (`.env`) for local API key shielding, backed by Firebase Remote Config as a secure cloud fallback.

## 3. Core Features

### A. The Prompt and Notes Screens & Smart AI Assistant
* **Personalized Context Awareness:** The AI dynamically injects the user's saved Firestore notes into the "System Prompt," allowing it to answer accurately based entirely on the user's specific data.
* **Voice-to-Text Integration:** Features native microphone integration utilizing `record` and `audioplayers`, allowing users to dictate prompts hands-free on both mobile and desktop environments.

### B. Advanced Search & Navigation
* **Instant Keyword Search:** Built-in search engine allowing users to find specific keywords across all notes instantly.
* **Dynamic Navigation:** A system that highlights search results and enables jumping directly between matching notes, mirroring the intuitive UI of modern messaging apps.

### C. Real-Time Cross-Platform Sync
* **Desktop & Mobile Harmony:** Users can edit or delete notes seamlessly on their Windows laptop, with the AI's "brain" and the Android app instantly updating to reflect the new data via Firestore real-time listeners.

## 4. Security & Privacy (Production Standards)
Security is a foundational pillar of this application:

* **Authentication:**
  * *Biometric Security Gate:* Mobile app access is locked behind fingerprint or FaceID authentication.
  * *Multi-Provider Login:* Secure authentication via Email/Password and Google OAuth.
* **Firestore Security Rules:** Strict, Identity-Based Rules. Users can only read and write documents that match their specific Google UID.
* **Local Secrets:** Sensitive API credentials are excluded from source control via `.gitignore` and `.env` implementations.

## 5. Resilience & Reliability
* **Offline Persistence:** Engineered with smart local caching. Users can open the app, read notes, and interact with the UI even in offline environments (like lecture halls). Changes are synced automatically to the cloud the moment the connection is restored.

---

## 🔒 Security & Source Code Notice

This repository is a public showcase of the Spark Pro architecture and AI integration capabilities. The proprietary source code, including the Gemini LLM API endpoints and Firebase configurations, is kept in a separate, private repository to ensure absolute security and protect intellectual property.

---

## 👤 Author

**Developed by Jana W. Seif**
*Biomedical Engineering | Cairo University*
* Bridging the gap between intelligent medical systems, IoT hardware, and human productivity.
* **GitHub:** [@janawaleed135](https://github.com/janawaleed135)
