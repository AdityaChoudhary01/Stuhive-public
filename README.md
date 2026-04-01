# 📑 StuHive: The Cinematic Academic Discovery Engine

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-15-000?style=for-the-badge&logo=next.js&logoColor=white" />
  <img src="https://img.shields.io/badge/React-19-61dafb?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Infrastructure-Cloudflare%20R2-f38020?style=for-the-badge&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-Azure%20Cosmos-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white" />
</p>

<div align="center">
  <h3><strong>Empowering students through decentralized, open-access knowledge sharing.</strong></h3>
  <p>StuHive is a high-performance, cinematic academic library designed to transform static study materials into a dynamic, real-time discovery experience.</p>
  
  <a href="https://www.stuhive.in"><b>🌐 Live Website</b></a> •
  <a href="https://www.stuhive.in/search"><b>🔍 Discovery Engine</b></a> •
  <a href="https://www.stuhive.in/blogs"><b>✍️ Insights Blog</b></a> •
  <a href="https://www.stuhive.in/supporters"><b>🏆 Wall of Fame</b></a>
</div>

---

## 📱 The Mobile Experience (Native Power)

> [!IMPORTANT]
> **🚀 StuHive Android APK is now available for direct download!**
> Experience the full power of the Hive with native performance, push notifications, and high-spec PDF rendering.
> 
> [<img src="https://img.shields.io/badge/Download-Android%20APK-00C853?style=for-the-badge&logo=android&logoColor=white" />](https://github.com/AdityaChoudhary01/Stuhive-public/releases/download/v1.1.0/StuHive.apk) *(Download the latest Production APK)*

### 🌓 Cross-Platform Synergy
- **Deep Linking**: Share a link on WhatsApp, and it opens the specific note instantly in the App.
- **Biometric Ready**: Secure access to your academic wallet and purchased notes.
- **Offline Sync**: Study your saved collections even without an active data connection.

---

## 🗺️ Live Platform Modules (Backlinks)

Explore the specialized sectors of the StuHive ecosystem:

| Module | Core Functionality | Official Link |
| :--- | :--- | :--- |
| **Academic Hubs** | Specialized pages for 500+ Universities & Boards. | [Visit Hubs](https://www.stuhive.in/hub) |
| **Global Search** | Hyper-fast, relevance-based cross-platform search. | [Search Hive](https://www.stuhive.in/global-search) |
| **Student Wallet** | Manage earnings from note sales and premium access. | [Go to Wallet](https://www.stuhive.in/wallet) |
| **Leaderboard** | Real-time ranking of top contributors and educators. | [View Rankings](https://www.stuhive.in/leaderboard) |
| **Legal Portal** | Industry-standard Privacy, Terms, and DMCA protocols. | [Legal Info](https://www.stuhive.in/privacy) |

---

## 🏗️ Technical Infrastructure (The Hardened Stack)

StuHive is built using a **ruthless performance methodology**, optimized for maximum scale on free-tier infrastructure (Azure/Vercel).

### 🏎️ 1. Incremental Static Regeneration (ISR)
We utilize **Next.js ISR** to serve content at the edge. 
- **Latency**: Time-to-First-Byte (TTFB) is reduced to **<30ms**.
- **Scale**: A single database request can serve **10,000+ users**, protecting our Azure Cosmos DB from connection exhaustion.

### 🛡️ 2. Self-Healing Database Pattern
Designed for the **Azure Cosmos DB vCore** ecosystem, our database layer features:
- **Connection Heartbeats**: Automatic reconnection logic that handles `ECONNRESET` instantly.
- **Optimized Pooling**: `maxPoolSize: 1` per serverless instance to maximize concurrent user capacity.
- **ReadyState Guards**: Every query is gated by a connectivity check, ensuring 99.9% uptime.

### 🔐 3. Intelligence Identity Layer
- **Auth Caching**: Implemented a **10-second identity cache** for mobile API requests, reducing redundant database lookups by 60%.
- **Secure Persistence**: Hybrid session management across Web (NextAuth) and Mobile (JWT/SecureStore).

---

## ✨ Key Features & Innovation

### 💬 Real-Time Mesh
Powered by **Ably WebSockets**, our chat system features:
- **Presence Tracking**: Real-time Online/Offline status indicators.
- **Unread Counters**: Dynamic badges synchronized across all devices.
- **Portal Rendering**: Chat dialogues occupy a separate DOM layer for 0% layout shift.

### 📚 The Academic Vault
- **Cloudflare R2**: Secure, s3-compatible storage with **Zero Egress Fees**, allowing unlimited downloads for students.
- **Optimistic UI**: Notes are "saved" or "collected" instantly in the UI while the background syncs with the DB.

### 🔍 Discovery Engine (High-Octane SEO)
- **JSON-LD Injection**: Automated Schema.org schema for every note, blog, and university hub to secure Google Rich Snippets.
- **Dynamic Meta Engine**: Scalable metadata generation that updates in real-time as your library grows.

---

## 📂 Architecture Overview

```text
├── actions/             # Server Actions (Secure DB mutations)
├── app/                 # Next.js 15 App Router (ISR Enabled)
│   ├── (hub)/           # University Central Nervous System
│   ├── (marketplace)/   # Note Discovery & Transactions
│   └── api/mobile/      # Specialized High-Speed Mobile API
├── components/          # Premium UI Layer (Shadcn + Framer)
├── lib/                 # The Hardened DB & Auth Core
├── public/              # Service Worker & PWA Assets
└── models/              # Normalized MongoDB Schemas
```

---

## 🌟 The 2026 Vision (Roadmap)

- [x] **Project Genesis**: Next.js 15 & MongoDB Foundation.
- [x] **Real-time Era**: Ably WebSocket Integration & Global Chat.
- [x] **Native Launch**: Production-Grade Expo Android APK.
- [x] **ISR Overhaul**: Blazing fast <30ms page loads.
- [ ] **AI Note Architect**: Automated summarization of 100+ page PDFs.
- [ ] **Decentralized Boards**: Student-governed moderation systems.

---

## 🤝 Contributing & Legal

Contributions are what make the academic community incredible. If you have a suggestion, feel free to fork the repo and create a pull request.

**Owner**: Aditya Choudhary  
**License**: Distributed under the MIT License.  
**Contact**: [support@stuhive.in](mailto:aadiwrld01@gmail.com)

<p align="center">
  <br />
  <b>StuHive</b> — <i>Reinventing the way the world learns.</i>
</p>
