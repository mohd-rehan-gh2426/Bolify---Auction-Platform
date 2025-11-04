# 🏷️ Bolify - An Auction Platform

A full-featured **Auction Platform** built using the **MERN Stack (MongoDB, Express.js, React, Node.js)** that allows multiple user roles — **Auctioneers**, **Bidders**, and a **Super Admin** — to interact in a seamless, real-time auction environment.

---

## 🚀 Features Overview

The platform enables real-time online auctions with transparent bidding, commission management, and admin oversight.  

There are three main user roles:

1. **Auctioneer** → Creates and manages auctions  
2. **Bidder** → Participates in live auctions  
3. **Super Admin** → Monitors and manages the entire platform  

---

## 🧑‍💼 User Roles and Flows

### 🧰 1. Auctioneer Flow

- **View Featured Auctions**  
  Can explore all currently running or featured auctions on the platform.

- **Create Auction**  
  Auctioneers can create new auctions by providing:
  - Title  
  - Category  
  - Condition  
  - Starting Bid  
  - Description  
  - Auction Start & End Time  
  - Item Image  

- **View Leaderboard**  
  See the leaderboard displaying top bidders who have won the most auctions.

- **Submit Commission (Key Feature)**  
  - When an item is sold, the auctioneer must pay a **5% commission** of the winning bid to the Super Admin.  
  - The auctioneer uploads:
    - **Payment Amount**
    - **Screenshot / Proof of Online Payment**
  - The **Super Admin** reviews and approves the commission.
  - **Note:** Until pending commissions are settled, the auctioneer **cannot create new auctions.**

- **View My Auctions**  
  Manage and review all auctions created — both ongoing and completed.

---

### 💰 2. Bidder Flow

- **Browse Featured Auctions**  
  View all running and featured auctions available for bidding.

- **Place Bids**  
  - Bidders must place a bid higher than the **current highest bid**.
  - Cannot bid on **ended auctions**.
  - Bidding logic ensures fair competition and proper price increments.

- **Winning Notification**  
  - Once an auction ends, the **winner receives an email** notifying them of their success.  
  - The email includes the **auctioneer’s bank/payment details**, allowing both parties to handle payment directly and mutually.

---

### 🛡️ 3. Super Admin Flow

- **Approve Commissions**  
  - Reviews commissions submitted by auctioneers.
  - Can approve or reject commission requests.

- **Manage Auctions**  
  - View all auctions created across the platform.
  - Delete inappropriate or invalid auctions.
  - Maintain platform integrity and compliance.

---

## ⚙️ Tech Stack

**Frontend:**
- React.js  
- Tailwind CSS (for UI styling)  
- Axios (for API communication)  
- React Router DOM  

**Backend:**
- Node.js  
- Express.js  
- MongoDB with Mongoose  
- Cloudinary (for image uploads)  
- JWT Authentication  
- Nodemailer (for email notifications)

---

## 📦 Project Setup

### Clone Repository
```bash
git clone https://github.com/your-username/mern-auction-platform.git
cd mern-auction-platform
