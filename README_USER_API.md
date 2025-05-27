# User API (Change Email)

Production-ready Flask API for user registration, login, and secure email change — all in one project.  
Includes JWT authentication, rate-limiting, Docker, SQLite, .env, and clean modular code.

---

## 🚀 Features

- Change email (JWT protected)
- Email validation & duplicate check
- Rate limiting (anti-bruteforce)
- Docker & .env support, SQLite out of the box
- Clean structure, production-ready, all-in-one

---

## 📦 Endpoints
---

### POST `/change-email` (JWT protected)

**Headers:**  
Authorization: Bearer <JWT>

**Request:**
```json
{
  "new_email": "newuser@example.com"
}
```

**Response:**
```json
{
  "message": "Email updated successfully"
}
```

---

## ⏱️ Rate limits

- `/register`: 5 per hour
- `/login`: 10 per hour
- `/change-email`: 5 per hour

---

## ⚡ Quick Start

### Docker (recommended)
```bash
docker build -t user-api .
docker run -d -p 5000:5000 user-api
```

### Local
```bash
pip install -r requirements.txt
python app.py
```

### .env example
```
JWT_SECRET_KEY=your-jwt-secret-here
DATABASE_URI=sqlite:///users.db
```

---

## 🖼️ Screenshots
- Server running
- Postman: change-email

---

## 📬 Contact

**Need this in another stack (Node.js, Go, etc)?**  
Contact: talabov.ali72@gmail.com  
Telegram: [@talabovali](https://t.me/talabovali)

*Note: Pricing may vary depending on complexity and target stack.*

---

**Ready for production and monetization. 100% tested.**
