# 🚀 ReceiptIQ Backend — AI-Powered Finance Management API

ReceiptIQ Backend is a scalable AI-powered financial management API that helps users scan receipts, track expenses, manage savings goals, and interact with an intelligent financial assistant using Generative AI.

Built with a modular architecture using **Node.js**, **Express.js**, **TypeScript**, **Prisma**, and **PostgreSQL**.

---

# ✨ Unique Features

## 🤖 AI-Powered Receipt Scanning
Uses OCR and Generative AI (Gemini/OpenAI) to automatically extract merchant names, total amounts, and itemized expenses from receipt images.

## 🎙️ Voice-to-Expense
Users can add expenses naturally using voice commands, which are processed and categorized using AI.

## 🎯 Intelligent Goal Tracking
Create financial goals and receive AI-generated budget advice and saving strategies.

## 📅 Subscription Detection
Automatically detects recurring subscriptions from spending behavior.

## 🛡️ Robust Admin Panel
Manage users, monitor AI usage, control system settings, and enable maintenance mode.

## 🔐 Enterprise-Grade Authentication
Secure authentication and session management powered by Better-Auth.

## 📈 AI Usage Monitoring
Tracks AI API usage, request logs, and system performance for monitoring and analytics.

---

# 🏗️ Project Structure

```bash
src/
├── app/
│   ├── config/             # Environment, database & cloud configs
│   ├── lib/                # Prisma, Cloudinary & third-party setups
│   ├── middlewares/        # Auth, error handling & global middlewares
│   ├── modules/            # Feature-based modular architecture
│   │   ├── auth/           # Authentication & session management
│   │   ├── chat/           # AI financial assistant
│   │   ├── goal/           # Savings goals & AI budget advice
│   │   ├── receipt/        # Receipt scanning & expense tracking
│   │   └── user/           # User management
│   ├── routes/             # API route aggregation
│   ├── templates/          # EJS email templates
│   ├── utils/              # Utility helpers & constants
│   └── views/              # Optional static views
│
├── app.ts                  # Express app configuration
└── server.ts               # Application entry point
```

---

# ⚙️ Tech Stack

| Category | Technology |
|---|---|
| Runtime | Node.js |
| Framework | Express.js v5 |
| Language | TypeScript |
| Database | PostgreSQL |
| ORM | Prisma |
| AI Integration | Google Gemini, OpenAI, Groq |
| Authentication | Better-Auth |
| Media Storage | Cloudinary |
| Logging | Winston |
| Email Service | Nodemailer |

---

# 🚀 Getting Started

## 1️⃣ Prerequisites

Before running the project, make sure you have:

- Node.js (v18+ recommended)
- PostgreSQL Database
- Cloudinary Account
- Gemini / OpenAI / Groq API Keys

---

## 2️⃣ Installation

Clone the repository and install dependencies:

```bash
npm install
```

---

## 3️⃣ Environment Variables

Create a `.env` file in the root directory and add the following:

```env
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/receiptiq"

# AI Keys
GEMINI_API_KEY="your_gemini_key"
GROQ_API_KEY="your_groq_key"
OPENAI_API_KEY="your_openai_key"

# Cloudinary
CLOUDINARY_CLOUD_NAME="your_cloud_name"
CLOUDINARY_API_KEY="your_api_key"
CLOUDINARY_API_SECRET="your_api_secret"

# Authentication
BETTER_AUTH_SECRET="your_secret"
BETTER_AUTH_URL="http://localhost:5000"

# Email
EMAIL_USER="your_email"
EMAIL_PASS="your_app_password"
```

---

## 4️⃣ Database Setup

Generate Prisma Client and sync the schema:

```bash
npm run generate
npm run push
```

---

## 5️⃣ Run Development Server

```bash
npm run dev
```

Server will run on:

```bash
http://localhost:5000
```

---

# 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/v1/auth/signup` | Register a new user |
| POST | `/api/v1/receipts/scan` | Scan receipt image with AI OCR |
| POST | `/api/v1/receipts/voice` | Add expense using voice |
| POST | `/api/v1/goals/create` | Create a savings goal |
| GET | `/api/v1/goals/:id/ai-advice` | Get AI-generated financial advice |
| GET | `/api/v1/chat` | Chat with AI financial assistant |

---

# 📌 Highlights

- Modular scalable backend architecture
- AI-powered financial automation
- Secure session-based authentication
- Cloud image upload support
- AI usage logging & monitoring
- RESTful API design
- Type-safe backend with Prisma & TypeScript

---

# 📝 License

This project is licensed under the ISC License.

---

# ❤️ Contest Submission

Built with passion for the contest submission using modern AI-powered technologies.
