📌 Overview

This Next.js application automates email ingestion, fetching emails via IMAP, POP3, Gmail API, and Outlook to extract PDF attachments. It stores email data and attachments locally and in a PostgreSQL database using Prisma ORM. The app ensures seamless data flow, real-time processing, and high scalability.

🔥 Features

Automated Email Fetching: Supports IMAP, POP3, Gmail API, and Outlook.

PDF Extraction: Detects and saves PDF attachments.

Database Integration: Uses PostgreSQL with Prisma ORM.

Next.js API Routes: Handles data processing efficiently.

Error Handling: Provides robust logging and validation.

Dynamic UI: Built with React & TailwindCSS for smooth UX.

🛠 Tech Stack

Framework: Next.js (React, TypeScript)

Backend: Node.js, Next.js API Routes

Database: PostgreSQL, Prisma ORM

Email Integration: IMAP, POP3, Gmail API, Outlook API

Styling: TailwindCSS

Authentication: NextAuth.js (if implemented)

🚀 Installation & Setup

1️⃣ Clone the Repository


2️⃣ Install Dependencies

npm install  # or yarn install

3️⃣ Configure Environment Variables

Create a .env file and add:

4️⃣ Run Migrations

npx prisma migrate dev --name init

5️⃣ Start the Application

npm run dev  # or yarn dev

📡 API Endpoints

Method

Endpoint

Description

POST

/api/email-ingestion

Fetch emails and store attachments

GET

/api/emails

Retrieve stored emails from DB

📄 Folder Structure

📂 email-pdf-ingestion
├── 📂 src
│   ├── 📂 app
│   │   ├── 📂 api
│   │   │   ├── 📂 email-ingestion
│   │   │   │   ├── route.ts
│   ├── 📂 components
│   ├── 📂 utils
│   ├── 📜 page.tsx
├── 📂 prisma
│   ├── schema.prisma
├── 📜 next.config.js
├── 📜 package.json
├── 📜 README.md

📌 Contributing

Fork the repo.

Create a new branch (feature/new-feature).

Commit changes and push.

Open a pull request.

📄 License

This project is licensed under the MIT License.
