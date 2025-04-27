# 📬 Contact Backend (Node.js + Express + Nodemailer)

This is a secure backend service built with **Node.js**, **Express**, and **Nodemailer** to handle contact form submissions from a portfolio website.  
It receives form data (name, email, message) and sends it to your email address securely.

## 🚀 Tech Stack
- Node.js
- Express.js
- Nodemailer
- dotenv
- CORS

## ⚙️ Environment Variables (`.env`)
Create a `.env` file in the project root with the following:
```env
PORT=5000
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
```

## 🛠 Setup Instructions (Local Development)
1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/contact-backend.git
cd contact-backend
```

2. **Install dependencies:**
```bash
npm install
```

3. **Create `.env` file** in the root (as shown above).

4. **Start the server:**
```bash
node index.js
```

Server runs on:  
```
http://localhost:5000
```

## 📬 API Endpoint

| Method | Endpoint            | Description               |
|:------:|:--------------------|:---------------------------|
| POST   | `/send-email`        | Send email from contact form |

### Request Body (JSON):
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "message": "Hello! This is a test."
}
```

## 🌍 Deployment (on Render)
1. Push this backend to a **new GitHub repository**.
2. Go to [Render.com](https://render.com).
3. Click **New +** → **Web Service** → Connect your GitHub repo.
4. Set:
   - **Build Command:** `npm install`
   - **Start Command:** `node index.js`
   - **Environment:** `Node`
5. Add environment variables in Render dashboard (`EMAIL_USER`, `EMAIL_PASS`, `PORT`).

6. Deploy!

You will get a public URL like:
```text
https://contact-backend.onrender.com
```

Update your React frontend to use this URL when making API requests.

## 🔐 Security Best Practices
- Never push `.env` file to GitHub.
- Always use `App Passwords` for Gmail SMTP.

## 👨‍💻 Author
- **Soniya Devikar**
- [https://github.com/soniyadevikar]

## 📜 License
This project is licensed under the MIT License.