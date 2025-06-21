#Store Mitra

**Store Mitra** is a smart, mobile-first inventory and sales management app built for small retail store owners in India. With built-in analytics, restocking insights, and ad monetization, Store Mitra acts as a pocket business partner — streamlining daily tasks while helping stores grow smarter.

---

## ✨ Features

### 🔐 User Authentication (via Firebase)
- Email/password signup and login
- Store name captured during account creation
- Auth state routing — app only accessible after login
- User profile saved in Firebase Firestore
- Persistent cloud sync for each authenticated user

### 📦 Inventory & Business Management
- Add restock entries (unit and case based)
- Auto-calculate total wholesale/retail/profit
- View restock history in detailed cards
- Manage expenses with breakdown
- Sales tracking with revenue computation
- Price list editable per product
- Business reports: weekly/monthly/yearly profit stats

### 📊 Business Analytics
- Smart dashboard showing:
  - Today’s sales
  - Expenses
  - Net profit
- Reports for trends over time
- Future-ready for AI suggestions (coming soon)

### 📱 Mobile-Optimized UX
- PWA-friendly responsive design
- Capacitor-based Android APK support
- Bottom navigation for mobile ease

### 💰 Ad Monetization (AdMob)
- AdMob SDK integration
- Banner ads show only on mobile devices
- Test ads supported in dev mode
- Error handling and fallback support

---

## 🧰 Tech Stack

| Layer          | Technology                          |
|----------------|-------------------------------------|
| Frontend       | React + TypeScript + Vite           |
| Routing        | Wouter (lightweight React router)   |
| State/Query    | React Query (@tanstack/react-query) |
| Backend        | Node.js + Express                   |
| Mobile         | CapacitorJS (for Android builds)    |
| Auth/DB        | Firebase Auth + Firestore           |
| Ads            | Google AdMob (mobile banner ads)    |
| Styling        | Tailwind CSS                        |

---

## 📁 Folder Structure (Client)
client/
├── public/
├── src/
│ ├── components/
│ ├── pages/
│ ├── hooks/
│ ├── lib/
│ ├── App.tsx
│ ├── main.tsx
│ └── index.css
└── package.json
---

## ⚙️ Setup Instructions

### 1. Clone the Repo
```bash
git clone https://github.com/tabz79/StoreMitra.git
cd StoreMitra
2. Install Dependencies
bash
Copy code
cd client
npm install
3. Firebase Setup
Create a Firebase project

Enable Email/Password auth

Create Firestore database

Add your Firebase config in src/lib/firebase.ts

ts
Copy code
// src/lib/firebase.ts
export const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_APP.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  ...
};
4. Run the Dev Server
bash
Copy code
npm run dev
App runs at http://localhost:5000

📦 Build & APK Generation (Android)
Install Capacitor:

bash
Copy code
npm install @capacitor/core @capacitor/cli
npx cap init "Store Mitra" "com.yourdomain.storemitra"
Add Android Platform:

bash
Copy code
npx cap add android
Sync and Open Android Studio:

bash
Copy code
npm run build
npx cap copy
npx cap open android
Build APK inside Android Studio.

🔮 Roadmap
 Firebase user auth

 AdMob integration

 LocalStorage sync

 Cloud sync for inventory/sales data

 AI-powered restock suggestions

 Multi-store management

 Dark mode toggle

 Language localization (Hindi, Telugu, etc.)

🙏 Acknowledgements
Firebase

React Query

CapacitorJS

Vite

Tailwind CSS

Google AdMob

📬 Contact
Built with ❤️ by @tabz79

DM for collaborations, contributions, or feature requests.

yaml
Copy code

---

Let me know if you'd like me to:
- Split into multiple sections like CONTRIBUTING.md or INSTALL.md
- Add screenshots or GIFs
- Include environment variable example file (e.g., `.env.example`)
