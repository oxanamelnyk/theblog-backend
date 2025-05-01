
# 🧠 Strapi Backend – Blog CMS

This is the **backend** for the [Next.js Blog Project](https://github.com/comoartista/theblog), built with **Strapi CMS**. It provides a REST API for managing and delivering blog content.

---

## 🔧 Tech Stack

- **CMS**: Strapi v5
- **Database**: PostgreSQL (on Railway)
- **Authentication**: API tokens, JWT
- **Media**: Uploads stored on server

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/comoartista/theblog-backend
cd theblog-backend
npm install
```

### 2. Create `.env` file

Create a `.env` file in the root:

```env
APP_KEYS=your_app_key_1,your_app_key_2
JWT_SECRET=your_jwt_secret
ADMIN_JWT_SECRET=your_admin_jwt_secret
API_TOKEN_SALT=your_api_token_salt
DATABASE_URL=your_postgresql_connection_url
```

> Use `node -e "console.log(require('crypto').randomBytes(32).toString('base64'))"` to generate secure values.

### 3. Run locally

```bash
npm run develop
```

By default, the admin panel runs at `http://localhost:1337/admin`

---

## 🌐 Production

The backend is deployed on **Railway**:  
🔗 [https://theblog-backend-production.up.railway.app](https://theblog-backend-production.up.railway.app)

Make sure CORS is enabled for your frontend domain.

---

## 📦 API Endpoints

Example:

```http
GET /api/posts
```

---

## 🔗 Related

Frontend repo:  
👉 [comoartista/theblog (Next.js frontend)](https://github.com/comoartista/theblog)
