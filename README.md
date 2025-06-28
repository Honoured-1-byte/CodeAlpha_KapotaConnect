
---

### 📱 **Task 2: KapotaConnect – Mini Social Media Platform**  
```markdown
# 📱 KapotaConnect – Mini Social Media App

A lightweight social network built for CodeAlpha’s internship.  
KapotaConnect supports user profiles, posts with comments, and follow/unfollow.

---

## 📌 Project Overview

**Tech Stack:**  
* Node.js & Express.js  
* EJS templating  
* SQLite (`sqlite3`) or MySQL (`mysql2`)  
* Multer + Cloudinary (for avatars)  
* express-session & Passport.js  

**Developer:** Honoured OneByte  
**Duration:** Internship Task 2

---

## ✨ Features

* **User Profiles**  
  * Register/login  
  * Avatar upload  

* **Posts & Comments**  
  * Create/delete text (& image) posts  
  * Comment on any post  

* **Follow System**  
  * Follow/unfollow other users  
  * View follower & following counts  

---

## 🚦 Routes

| Method | Path                   | Description               |
| ------ | ---------------------- | ------------------------- |
| GET    | `/`                    | Feed: all posts           |
| GET    | `/register`            | Signup form               |
| POST   | `/register`            | Handle signup             |
| GET    | `/login`               | Login form                |
| POST   | `/login`               | Handle login              |
| GET    | `/logout`              | Logout                    |
| GET    | `/profile/:username`   | User profile page         |
| GET    | `/post/new`            | New post form             |
| POST   | `/post/new`            | Create post               |
| GET    | `/post/:id`            | View post & comments      |
| POST   | `/post/:id/comment`    | Add comment               |
| POST   | `/follow/:userId`      | Follow user               |
| POST   | `/unfollow/:userId`    | Unfollow user             |

---

## 🛠️ Installation

```bash
# 1. Clone
git clone https://github.com/Honoured-1-byte/CodeAlpha_KapotaConnect.git
cd CodeAlpha_KapotaConnect

# 2. Install deps
npm install

# 3. Configure .env
cp .env.example .env
# fill DATABASE_URL, SESSION_SECRET, PORT

# 4. (Optional) Seed users
# node seedUsers.js

# 5. Start
npm start
