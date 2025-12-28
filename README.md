# FixIt Forge 🛠️  
### Home Repair & DIY Q&A Forum (3-Tier Architecture)

FixIt Forge is a themed question-and-answer forum focused on **home repair and DIY troubleshooting**.  
Users can register, log in, browse repair topics, ask questions, and post answers.

This project demonstrates a **3-Tier Architecture** using:
- **MongoDB** (Data Layer)
- **Node.js + Express** (Application Layer / JSON API)
- **React** (Presentation Layer / Single Page Application)

---

## 🚀 Features

- User registration & login (JWT authentication)
- Topic-based discussion hierarchy
- Ask and answer questions
- Mark answers as accepted (solved questions)
- Protected routes for authenticated users
- RESTful JSON API
- Seed data for demo purposes
- Initial setup
- Authentication
- Database Layer

---

## 🧱 3-Tier Architecture Overview

### 1. Data Layer (MongoDB)
Stores users, topics, questions, and answers.

### 2. Application Layer (Node.js + Express)
Handles:
- Authentication
- Business logic
- Database access
- JSON API responses

### 3. Presentation Layer (React SPA)
Client-side application that:
- Communicates with the API using JSON
- Displays topics, questions, and answers
- Allows authenticated user interactions

---

## 🗂️ Topic Hierarchy

- **Electrical**
  - Outlets & Switches
  - Lighting
- **Plumbing**
  - Leaks
  - Water Heaters
- **Appliances**
  - Washer / Dryer
  - Refrigerator
- **Tools & Safety**
  - Tool Advice
  - Safety & PPE

---

## 📊 Database Schema (MongoDB)

### Users
```js
{
  _id,
  username,
  email,
  passwordHash,
  role,
  createdAt
}
