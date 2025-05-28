# Imagify 🖼️✨

**Imagify** is an AI-powered image generation web app that allows users to create images from text prompts. It uses **ClipDrop AI** for image generation, **Clerk** for user authentication, and **Razorpay** for managing payments and purchasing credits.

---

## 🌟 Features

- 🔐 User authentication using Clerk (login/signup/logout)
- 🎨 AI-based image generation using ClipDrop
- 💳 Payment integration with Razorpay to buy credits
- 💼 Credit system for controlling image generation usage
- 🔧 Frontend + Backend architecture

---

## 🛠️ Tech Stack

- **Frontend:** Next.js, Tailwind CSS
- **Backend:** Node.js / Express (or your backend framework)
- **AI API:** ClipDrop
- **Authentication:** Clerk
- **Payments:** Razorpay

---

## ⚙️ Environment Variables

### 🔑 Server `.env`

```env
CLIPDROP_API_KEY=your_clipdrop_api_key
RAZORPAY_KEY_ID=
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
JWT_SECRET=your_jwt_secret
MONGODB_URI=your_mongodb_connection_string
```
### 🔑 Client `.env`

```env
VITE_BACKEND_URL = your_backend_url
VITE_RAZORPAY_KEY_ID = your_razorpay_key_id
```

## 🚀 How to Run the Project

### 📦 Prerequisites

- Node.js (v16+)
- npm or yarn
- MongoDB instance (local or Atlas)
- Clerk account (for authentication)
- Razorpay account (for payment processing)
- ClipDrop API key

---

### 🔧 Step 1: Clone the Repository

```bash
git clone https://github.com/Kreshipatel/Imagify.git
cd imagify

🔙 Step 2: Setup and Run the server
cd server
npm install
npm run server
Server will run at http://localhost:5000

🎨 Step 3: Setup and Run the Frontend

cd ../client
npm install
npm run dev
Frontend will run at http://localhost:5173

💬 How It Works
User signs in using Clerk.
Enters a text prompt to generate an image.
Backend sends the prompt to the ClipDrop API.
Generated image is returned and displayed.
User can purchase more credits via Razorpay.

📸 Example Prompt
"A majestic lion wearing sunglasses in a neon-lit jungle"
