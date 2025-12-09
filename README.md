# SkillSet – Freelance Service Marketplace Platform

SkillSet is a full-stack MERN application that connects employers with skilled professionals.  
Users can browse gigs, hire workers, communicate through an internal messaging system, and complete payments via Stripe — all inside a modern, responsive UI.

---

## 🚀 Features

### 👥 Dual Login System  
SkillSet supports two user roles:

#### **1. Employer**
- Browse available gigs  
- Hire workers  
- Send & receive messages with the hired employee  
- Manage active and completed jobs  
- Make secure payments using Stripe  

#### **2. Employee (Service Provider)**
- Create, edit, and delete gigs  
- Upload gig images (Cloudinary)  
- Receive orders from employers  
- Chat with the employer for confirmed jobs  
- Manage job status & earnings  

---

## 💬 Messaging System (MongoDB)
- Real-time-like messaging implementation using MongoDB  
- Messages stored securely in a `messages` collection  
- Only available **after a job is confirmed**  
- Clean chat UI for employer ↔ employee communication  

---

## 💳 Payment Integration (Stripe)
SkillSet includes full Stripe integration:
- Secure checkout  
- Tokenized payment flow  
- Employer → Employee payment routing logic  
- Verification & order creation after payment success  

---

## 🖼️ Image Storage (Cloudinary)
- All gig images are uploaded to Cloudinary  
- Optimized URLs stored in MongoDB  
- Faster load time & responsive images  

---

## 📦 Tech Stack

### **Frontend**
- React.js  
- React Router  
- Context API / Redux (based on your version)  
- TailwindCSS / Custom CSS  

### **Backend**
- Node.js  
- Express.js  
- MongoDB + Mongoose  

### **Other Tools**
- Stripe (Payment gateway)  
- Cloudinary (Image storage)  
- JWT (Auth)  
- bcrypt (Password hashing)  
- Axios (API requests)

---

## 📁 Project Structure (Simplified)

```
SkillSet/
│
├── client/                 
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   └── App.jsx
│   └── package.json
│
├── server/                 
│   ├── controllers/
│   ├── models/
│   │   ├── User.js
│   │   ├── Gig.js
│   │   ├── Order.js
│   │   └── Message.js
│   ├── routes/
│   ├── middlewares/
│   └── server.js
│
└── README.md
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository
```bash
git clone https://github.com/pranox/SkillSet.git
cd SkillSet
```

---

### 2️⃣ Install dependencies

#### Backend:
```bash
cd server
npm install
```

#### Frontend:
```bash
cd ../client
npm install
```

---

## 3️⃣ Configure Environment Variables

Create a `.env` file inside the **server** folder:

```
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
STRIPE_SECRET_KEY=your_stripe_key
CLOUDINARY_API_KEY=your_api_key

PORT=5000
```

---

## 4️⃣ Start the backend server
```bash
cd server
npm start
```

---

## 5️⃣ Start the frontend
```bash
cd client
npm run dev
```

---

## 📌 Future Improvements
- Push notifications for chat  
- In-app video/voice call  
- Advanced recommendation system  
- Employee performance ratings  

---

## 📜 License
MIT License  

---

## 🌟 About the Project
SkillSet was created as a full-stack learning project to implement real-world marketplace functionality including payments, messaging, authentication, and gig management using the MERN stack.

