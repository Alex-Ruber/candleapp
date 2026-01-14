🕯️ Candle

Candle is a mobile application that helps couples build and maintain emotional connection through small, consistent daily interactions.
The product is intentionally lightweight, private, and designed for long-term use.

Website: https://www.trycandle.app

📌 Overview

Candle focuses on consistency over intensity.
Daily interactions are designed to be completed in minutes, forming habits that compound over time.

The product avoids:

Public feeds

Social comparison

Pressure-driven gamification

🏗️ System Architecture
High-Level Architecture
+-------------------+
|   Mobile Clients  |
| (iOS / Android)   |
+---------+---------+
          |
          | HTTPS / REST
          |
+---------v---------+
|       API         |
|   (Node.js)       |
+---------+---------+
          |
          |
+---------v---------+
|    PostgreSQL     |
|     Database      |
+-------------------+

Component Breakdown
+--------------------------------------------------+
|                   Candle                         |
+---------------------+----------------------------+
| Mobile App          | Backend                    |
|---------------------|----------------------------|
| • Daily Prompts     | • Auth & Sessions          |
| • Photo Sharing    | • Prompt Engine             |
| • Micro Gestures   | • Partner Sync              |
| • Streak Tracking  | • Media Metadata            |
+---------------------+----------------------------+
             |
             |
+------------v------------+
|        Storage          |
|   (Images / Assets)     |
+-------------------------+

Daily Interaction Flow
User A opens app
        |
        v
Receives Daily Prompt
        |
        v
Completes Interaction
        |
        v
Prompt synced to partner
        |
        v
User B responds
        |
        v
Interaction archived

✨ Features
Daily Prompts

Lightweight prompts designed to encourage reflection, play, or conversation without pressure.

Shared Photo Moments

Private photo sharing that builds a contextual timeline of the relationship.

Micro-Interactions

Small gestures to signal presence, especially for long-distance or asynchronous use.

Streaks & Rituals

Subtle habit reinforcement without competition or comparison.

Local Date Ideas (Beta)

Contextual inspiration for offline connection.

🧠 Product Principles

Low friction — interactions take minutes

Private by default — no social graph

Intentional scope — features are narrow and focused

Emotional safety — no scoring or judgment

Long-term use — designed for months and years

🧩 Repository Structure
.
├── mobile/          # iOS & Android app
├── backend/         # API and business logic
├── web/             # Marketing site
├── docs/            # Internal documentation
├── .github/         # CI/CD workflows
└── README.md

🚀 Quick Start
Requirements

Node.js ≥ 18

npm or yarn

Xcode

Android Studio

Setup
git clone https://github.com/<org>/candle.git
cd candle
npm install


Create .env:

NODE_ENV=development
API_URL=http://localhost:3000


Run:

npm start

🧪 Testing
npm test


Includes unit and integration tests for:

Prompt flow

Partner sync

Media metadata

Streak logic

🔐 Security & Privacy

Private by default

No public profiles

No data resale or sharing

Report vulnerabilities to: security@trycandle.app

📄 License

MIT License.

🏢 Company

Candle is backed by Y Combinator and built by a small, product-focused team.
