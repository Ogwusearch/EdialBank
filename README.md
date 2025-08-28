# 🏦 Edial Bank

[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)  

**Edial Bank** is a full-featured educational banking web application with **customer and admin dashboards**, **real-time transactions**, **investment tracking**, and **secure authentication**. Built with **React**, **FastAPI**, and **PostgreSQL**, it demonstrates a modern **component-based architecture**, responsive UI, and secure banking flows.  

---

## 🌟 Features

### **Customer Features**
- User registration & login with JWT  
- Account overview dashboard with balance trends  
- **Investment overview cards**: track portfolios, stocks, or savings plans  
- View transaction history with filtering and export options  
- Fund transfers between accounts  
- Profile management (update personal info, password)  
- Real-time notifications and loading states  

### **Admin Features**
- Admin dashboard with system statistics  
- User management (add/edit/deactivate accounts, role assignment)  
- Transaction monitoring & analytics  
- Export reports (CSV/PDF)  
- Activity and audit logs  

### **UI/UX Features**
- Responsive design (mobile → desktop)  
- Professional banking color scheme  
- Loading spinners, error boundaries, and modals  
- Accessible and keyboard-friendly components  

### **Security Features**
- JWT authentication with HTTP-only cookies  
- Password hashing (bcrypt)  
- Input validation & sanitization  
- CSRF & XSS protection  
- Rate limiting and audit logging  

---

## 🧰 Tech Stack

| Layer           | Technology / Tool                        |
|-----------------|----------------------------------------|
| Frontend        | React 18 + Vite, React Router, MUI      |
| State Management| Context API, useReducer                  |
| Forms & Validation | React Hook Form + Yup                  |
| Charts/Analytics| Recharts / Chart.js                      |
| Backend         | FastAPI + SQLAlchemy + Pydantic         |
| Auth & Security | JWT, bcrypt, CSRF headers               |
| Database        | PostgreSQL / Supabase                     |
| Caching         | Redis                                    |
| Testing         | Jest, React Testing Library, Cypress     |
| DevOps/Hosting  | Docker, Docker Compose, Vercel/Render  |
| AI/ML (Optional)| Fraud detection, transaction categorization, predictive analytics |

---

## 📂 Project Structure

```

src/
├─ components/
│  ├─ Dashboard/
│  │  ├─ AccountCard.jsx
│  │  ├─ InvestmentCard.jsx       # Investment overview component
│  │  ├─ StatsCard.jsx
│  ├─ Admin/
│  │  ├─ AdminDashboard.jsx
│  │  ├─ UserManagement.jsx
│  │  ├─ SystemAnalytics.jsx
│  ├─ Shared/
│     ├─ LoadingSpinner.jsx
│     ├─ Notification.jsx
│     ├─ Modal.jsx
├─ pages/
│  ├─ auth/ (Login.jsx, Register.jsx)
│  ├─ customer/ (Dashboard.jsx, Transactions.jsx, Transfer.jsx, Profile.jsx)
│  ├─ admin/ (AdminDashboard.jsx, UserManagement.jsx, Analytics.jsx)
├─ contexts/ (AuthContext.jsx, ThemeContext.jsx, NotificationContext.jsx)
├─ hooks/ (useAuth.jsx, useAccounts.jsx, useTransactions.jsx, useInvestments.jsx)

````

---

## 🚀 Installation

### **Frontend**
```bash
git clone https://github.com/<your-username>/edial-bank.git
cd edial-bank/frontend
npm install
npm run dev
````

### **Backend**

```bash
cd ../backend
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows
pip install -r requirements.txt
uvicorn main:app --reload
```

### **Database**

* Install PostgreSQL / Supabase
* Create database `edial_bank`
* Run migrations or import seed JSON data

---

## ⚙ Usage

1. Open frontend: `http://localhost:5173`
2. Register or use demo credentials:

   * **Admin:** [admin@edialbank.local](mailto:admin@edialbank.local) / password
   * **Customer:** [user1@edialbank.local](mailto:user1@edialbank.local) / password
3. Explore dashboards, transactions, transfers, and investment cards
4. Admins can manage users and view analytics

---

## 🧪 Testing

### **Frontend**

```bash
npm test
```

### **Backend**

```bash
pytest
```

### **E2E**

```bash
npx cypress open
```

---

## 🔐 Security Notes

* Always use HTTPS in production
* JWT tokens are stored in HTTP-only cookies
* Input validation is enforced for all API endpoints
* Admin actions are logged for audit

---

## 📦 Deployment

* Docker Compose setup available for local dev
* Frontend can deploy to **Vercel** or **Netlify**
* Backend can deploy to **Render**, **Supabase Functions**, or **DigitalOcean App Platform**

---

## 📖 Contribution

Contributions are welcome!

* Fork the repo
* Create a feature branch (`git checkout -b feature/xyz`)
* Commit changes (`git commit -m 'Add feature xyz'`)
* Push branch and open a pull request

---

## ⚖ License

[MIT License](LICENSE)
