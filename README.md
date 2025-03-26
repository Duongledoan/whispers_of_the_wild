# 🌿 Whispers of the Wild - Wildlife Conservation Web App

## 📝 Project Overview
Whispers of the Wild is a **full-stack web application** designed to **raise awareness about wildlife conservation**, **attract new members**, and **showcase events, news, and conservation projects**. This application provides an interactive platform for users to learn about conservation efforts and upcoming events.

## 🏗 Tech Stack
### **Frontend:**
- HTML, CSS, JavaScript
- Responsive design with CSS Grid/Flexbox
- Fetch API for dynamic content loading

### **Backend:**
- Flask (Python)
- MongoDB Atlas (NoSQL Database)
- Flask-JWT-Extended (Authentication)
- Flask-CORS (Cross-Origin Requests Handling)

### **APIs Integrated:**
- Fetch wildlife-related news from external sources (e.g., WWF, Nature.org)

## 🌎 Features
### **1. Homepage (`index.html`)**
- Hero section with a mission statement
- Latest events preview
- News highlights
- Navigation links to key sections

### **2. Activities Page (`hoatdong.html`)**
- Grid layout showcasing conservation activities
- Clickable activity cards for more details

### **3. News Page (`news.html`)**
- Fetches and displays wildlife conservation news
- Uses an external API for dynamic content

### **4. Contact Page (`lienhe.html`)**
- Contact form with name, email, and message fields
- Displays club contact details and social media links

## ⚙️ Backend API Endpoints
### **News Management**
- `GET /api/news` → Fetch news articles from MongoDB (paginated)
- `POST /api/news` → Add a new news article (admin-only)
- `PUT /api/news/<article_id>` → Edit an existing article (admin-only)
- `DELETE /api/news/<article_id>` → Delete an article (admin-only)

### **Event & Activity Management**
- `GET /api/events` → Fetch events from MongoDB
- `POST /api/events` → Add an event (admin-only)
- `PUT /api/events/<event_id>` → Edit an event (admin-only)
- `DELETE /api/events/<event_id>` → Delete an event (admin-only)

### **Admin Authentication (JWT-based)**
- `POST /api/admin/login` → Authenticate admin and return a JWT token
- `GET /api/admin/dashboard` → Access admin dashboard (protected route)

### **Wildlife News API Integration**
- `GET /api/external-news` → Fetch external wildlife news

## 🗄 Database Schema (MongoDB Collections)
### **`news` Collection**
```json
{
  "_id": "ObjectId",
  "title": "Poaching Crisis in National Parks",
  "content": "Detailed article content here...",
  "image_url": "https://example.com/image.jpg",
  "created_at": "2025-03-15T10:00:00Z"
}
```
### **`events` Collection**
```json
{
  "_id": "ObjectId",
  "title": "Wildlife Awareness Workshop",
  "description": "Join us for an educational session on conservation.",
  "date": "2025-04-10",
  "image_url": "https://example.com/event.jpg"
}
```
### **`admins` Collection**
```json
{
  "_id": "ObjectId",
  "username": "admin123",
  "password_hash": "hashed_password_here",
  "role": "admin"
}
```

## 🚀 Getting Started
### **1️⃣ Backend Setup**
#### **Install Dependencies**
```bash
pip install flask flask-pymongo flask-jwt-extended flask-cors python-dotenv
```
#### **Set Up `.env` File**
```env
MONGO_URI=<your_mongodb_atlas_connection_string>
JWT_SECRET_KEY=<your_jwt_secret_key>
SECRET_KEY=<your_secret_key>
```
#### **Run the Flask App**
```bash
python app.py
```
Backend will be available at `http://localhost:5000`

### **2️⃣ Frontend Setup**
- Ensure `index.html`, `hoatdong.html`, `news.html`, and `lienhe.html` fetch data from the correct backend endpoints.
- Open `index.html` in a browser to start using the application.

## 🌐 Deployment
- Deploy **backend** to Render/Heroku with MongoDB Atlas
- Host **frontend** on Netlify or GitHub Pages

## 💡 Future Enhancements
- Add a **user registration system** for members
- Expand **news API integration** to more sources
- Improve **UI/UX design** with animations and interactivity

---
**Project Maintained By:** Whispers of the Wild Club 🌍🐾

