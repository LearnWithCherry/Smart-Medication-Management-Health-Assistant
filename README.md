# 💊 Smart Medication Management & Health Assistant

<div align="center">

![React](https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge&logo=react)
![Python](https://img.shields.io/badge/Backend-Python-3776AB?style=for-the-badge&logo=python)
![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=for-the-badge&logo=mysql)
![Tailwind CSS](https://img.shields.io/badge/UI-TailwindCSS-38B2AC?style=for-the-badge&logo=tailwind-css)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

### 🚀 A Full Stack Healthcare Management System with Real-World Data Structure Implementation

*"Managing medicines smarter, faster, and more efficiently."*

</div>

---

# Overview

Smart Medication Management & Health Assistant is a modern healthcare web application that helps users search medicines, receive AI-powered health guidance, request unavailable medicines, and manage personal medication history.

The project is specifically designed to demonstrate the practical implementation of **Data Structures & Algorithms (DSA)** in a real-world healthcare application while maintaining a modern Full Stack architecture.

---

# Features

## User Features

###  Smart Medicine Search

Search medicines using:

- Medicine Name
- Brand
- Disease
- Category

### 📦 Medicine Details

View complete medicine information including:

- 💰 Price
- 💊 Tablets per Strip
- 🩺 Uses
- 📖 Dosage
- 📅 Expiry Date
- 📦 Available Stock
- ⚠ Prescription Required
- 🏭 Manufacturer
- 🔄 Alternative Medicines

---

### 🤖 AI Health Assistant

Users can describe their symptoms:

> **Example**

```
I have fever and headache.
```

AI provides:

- Possible causes
- OTC medicine suggestions
- Home remedies
- Precautions
- Doctor consultation advice

> **Note:** This assistant provides recommendations only and does **NOT** replace professional medical advice.

---

### 📝 Medicine Request System

If a medicine is unavailable, users can submit a request:

- Medicine Name
- Quantity
- Contact Information
- Additional Notes

The request is automatically sent to the Admin Dashboard.

---

### 👤 User Profile

Users can access:

- Previous Searches
- Requested Medicines
- Saved Medicines
- AI Chat History

---

# 🛠 Admin Dashboard

## 📊 Dashboard Overview

- Total Medicines
- Total Requests
- Low Stock Alerts
- New Arrivals
- Most Selling Medicines
- Least Selling Medicines

---

## 📦 Inventory Management

Admin can:

- ➕ Add Medicine
- ✏ Update Stock
- 🗑 Delete Medicine
- 💰 Change Price
- 📅 Update Expiry Date

---

## 📋 Medicine Requests

Displays:

| User | Medicine | Quantity | Date | Status |
|------------|------------|------------|------------|------------|

Admin Actions:

- ✅ Approve
- ❌ Reject
- 🚚 Mark Ordered

---

## 📈 Sales Analytics

Interactive graphs showing:

- Top Selling Medicines
- Least Selling Medicines
- Monthly Sales
- Category Distribution

---

## ⏰ Expiry Tracker

Automatically identifies medicines expiring within:

- 30 Days
- 60 Days
- 90 Days

---

## 🤖 AI Insights

Provides intelligent suggestions:

- Medicines to Restock
- Fast Moving Inventory
- Slow Moving Inventory

---

# 🏗 Project Architecture

```
                 👤 User
                    │
                    ▼
         React + Tailwind Frontend
                    │
                    ▼
          Python REST API Backend
                    │
                    ▼
         Data Structure Processing Layer
                    │
                    ▼
              MySQL Database
```

---

# 💻 Tech Stack

| Layer | Technology |
|----------------|----------------------|
| Frontend | React.js |
| Styling | Tailwind CSS |
| Backend | Python (Flask / FastAPI) |
| Database | MySQL |
| AI Integration | Gemini / OpenAI API |
| API Testing | Postman |
| Version Control | Git & GitHub |

---

# 📂 Project Structure

```
Smart-Medication-Management/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── components/
│
├── backend/
│   ├── api/
│   ├── models/
│   ├── routes/
│   └── data_structures/
│
├── database/
│   ├── schema.sql
│   └── seed.sql
│
├── assets/
│
├── README.md
└── requirements.txt
```

---

# 🧠 Data Structures Implementation

This project demonstrates practical applications of multiple Data Structures.

---

## 1️⃣ Array

### Used For

- Medicine List
- Categories
- Search Results

```
Medicines[]

Paracetamol
Crocin
Dolo
```

### Complexity

```
Access : O(1)
Traversal : O(n)
```

---

## 2️⃣ Linked List

### Used For

Medicine Request Queue

```
Request 1
    ↓
Request 2
    ↓
Request 3
```

### Advantage

Efficient insertion and deletion.

```
Insertion : O(1)
Deletion : O(1)
```

---

## 3️⃣ Stack

### Used For

Recent Searches

```
Search A
Search B
Search C
──────────
Top → Search C
```

### Principle

```
LIFO
Last In First Out
```

---

## 4️⃣ Queue

### Used For

Admin Request Processing

```
User1
User2
User3
```

### Principle

```
FIFO
First In First Out
```

---

## 5️⃣ HashMap

### Used For

Instant Medicine Search

```
Paracetamol → Object

Crocin → Object

Dolo → Object
```

### Complexity

```
Search : O(1)
```

instead of

```
Linear Search : O(n)
```

---

## 6️⃣ Binary Search Tree (BST)

### Used For

Sorting by

- Price
- Stock
- Expiry Date

```
          500
        /     \
      300     700
```

### Complexity

```
Search : O(log n)
Insertion : O(log n)
```

---

## 7️⃣ Priority Queue (Heap)

### Used For

Expiry Alert System

```
Highest Priority

Medicine Expiring Tomorrow

↑

Medicine Expiring Next Week

↑

Medicine Expiring Next Month
```

### Complexity

```
Insert : O(log n)
Delete : O(log n)
```

---

## 8️⃣ Graph (Advanced)

Used for Medicine Recommendation Network

```
        Fever
          │
          ▼
    Paracetamol
          │
          ▼
     Pain Relief
          │
          ▼
        Crocin
```

Useful for AI-based medicine suggestions.

---

# 🗄 Database Schema

## Medicines

| Field |
|----------------|
| Medicine_ID |
| Name |
| Price |
| Stock |
| Tablets |
| Expiry |
| Uses |
| Category |
| Manufacturer |

---

## Users

| Field |
|----------------|
| User_ID |
| Name |
| Email |
| Password |
| Phone |

---

## Medicine Requests

| Field |
|----------------|
| Request_ID |
| User_ID |
| Medicine |
| Quantity |
| Status |

---

## Sales

| Field |
|----------------|
| Sale_ID |
| Medicine_ID |
| Quantity |
| Date |

---

# 🔗 REST APIs

## User APIs

```
GET    /medicine/search

GET    /medicine/:id

POST   /medicine/request

POST   /ai/assistant
```

---

## Admin APIs

```
GET    /admin/inventory

POST   /admin/addmedicine

PUT    /admin/updatestock

DELETE /admin/deletemedicine

GET    /admin/reports
```

---

# 🎨 UI Design Philosophy

✔ Minimal Interface

✔ Mobile Friendly

✔ Responsive Layout

✔ Card Based Design

✔ Large Search Bar

✔ Elderly Friendly Navigation

✔ Soft Color Palette

✔ Dark Mode Support

---

# ⚡ Time Complexity

| Operation | Data Structure | Complexity |
|--------------------------------|----------------|------------|
| Search Medicine | HashMap | **O(1)** |
| Process Request | Queue | **O(1)** |
| Recent Search | Stack | **O(1)** |
| Add Request | Linked List | **O(1)** |
| Sort by Expiry | BST | **O(log n)** |
| Expiry Alert | Priority Queue | **O(log n)** |

---

# 🌟 Future Enhancements

- 💳 Online Medicine Ordering
- 📍 Nearby Pharmacy Locator
- 📱 Mobile Application
- 🔔 Medicine Reminder Notifications
- 📄 Prescription Upload & OCR
- 📊 AI Health Analytics
- 🌐 Multi-language Support

---

# 🚀 Getting Started

```bash
# Clone Repository

git clone https://github.com/yourusername/smart-medication-management.git

# Frontend

cd frontend
npm install
npm run dev

# Backend

cd backend
pip install -r requirements.txt
python app.py
```

---

# 🤝 Contributing

Contributions, feature requests, and suggestions are welcome.

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push the branch
5. Open a Pull Request

---

# 📄 License

This project is created for **Educational & Academic Purposes** to demonstrate practical implementation of **Data Structures, Full Stack Development, and AI Integration**.

---

<div align="center">

## ⭐ If you like this project, don't forget to Star the Repository!

**Made with ❤️ using React, Python, MySQL & Data Structures**

</div>
