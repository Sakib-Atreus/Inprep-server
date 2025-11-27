# InPrep Server – AI Mock Interview

A scalable and modular backend for the **InPrep** platform — an AI-powered mock interview application.  
This server handles **user authentication, interview processing, resume parsing, Stripe payments, admin analytics, and content management**, built with modern best practices.

---

## 🚀 Features

### ✅ Authentication & User Management
- JWT-based login & registration  
- Token refresh + logout  
- Role-based access
- Secure password hashing  

### 🎙️ AI Mock Interview System
- Users select a topic & record/video interview  
- Speech-to-text transcript generation  
- AI analysis for:  
  - Confidence level  
  - Filler words  
  - Speaking clarity  
  - Final feedback score  
- Stores interview details in MongoDB  
- Admin can view all interviews  

### 📄 Resume Handling & Manual Input
- PDF resume upload (Cloudinary)  
- Resume extraction  
- Manual entry for **About Me** + **Experience**  
- Multi-step resume flow compatible with React frontend  

### 💳 Stripe Payment System
Supports three plans:
- **Free** → 1 interview  
- **Premium Subscription** → Unlimited interviews  
- **Pay-Per-Interview** → Buy interviews individually  

Includes:
- Stripe Checkout Session  
- Webhook to store payment results  
- Database integration with `Payment` model  
- Payment history in Admin Dashboard  

### 📊 Admin Dashboard APIs
- Total users  
- Total payments  
- Total interviews  
- Monthly revenue graph  
- Combined user + profile + payment views  
- Landing page content management with image upload  

### ☁️ File Upload (Cloudinary + Multer)
- Supports image uploads (logo, banner, section images)  
- Used in the Landing Page Content Management panel  

### 🧱 Tech Stack
- Node.js  
- Express.js  
- TypeScript  
- MongoDB + Mongoose  
- Stripe  
- Cloudinary  
- Modular Architecture  
- Zod Validation  

---

## 📁 Project Structure

```bash

src/
├── modules/
│ ├── auth/
│ ├── user/
│ ├── profile/
│ ├── interview/
│ ├── payment/
│ ├── resume/
│ ├── dashboard/
│ └── landing/
├── utils/
├── middleware/
├── config/
├── app.ts
└── server.ts

```

---

## 🛠️ Installation

```bash
git clone https://github.com/yourname/inprep-server.git
cd inprep-server
npm install
```

## ▶️ Run in Development

```bash
npm run dev
```

## 🏗️ Build

```bash
npm run build
```

## 🚀 Production

```bash
npm start
```

## 🎯 Future Enhancements

• AI real-time scoring

• Recommendation system for interview improvement

• Resume optimization using AI

• Multi-language support

## ⚠️ Copyright & Usage Warning

This project is the proprietary work of the InPrep team.

All code, logic, architecture, and content in this repository are protected.
