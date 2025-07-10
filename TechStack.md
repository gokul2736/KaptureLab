# 🔧 KaptureLab – Full Tech Stack & Tools



> This file documents the complete technical stack powering **KaptureLab**, from frontend to backend, database, authentication, analytics, and deployment.



## 🖥️ Frontend

| Tool/Library     | Purpose                                           |
|------------------|---------------------------------------------------|
| **HTML5**         | Page structure and layout                         |
| **CSS3**          | Styling and responsive design                     |
| **JavaScript (ES6)** | Dynamic behavior and user interaction         |
| **QRCode.js**     | Generate QR codes from GitHub repo links         |
| **html2pdf.js**   | Convert HTML lab records into downloadable PDFs  |
| **LocalStorage**  | Store guest session data temporarily             |



## 🔐 Authentication & Authorization

| Tool/Service        | Purpose                                      |
|---------------------|----------------------------------------------|
| **Firebase Auth**    | Login via Google and session management     |
| **GitHub OAuth App** | Login via GitHub + repo access              |
| **OAuth 2.0 Flow**   | Secure token exchange from GitHub           |
| **User UID System**  | Unique identity used across Firestore/Storage |



## ☁️ Backend Logic & Cloud Functions

| Tool                | Purpose                                        |
|---------------------|------------------------------------------------|
| **Firebase Functions** | Serverless backend logic                   |
| `getGitHubAccessToken()` | Exchange GitHub code for access token    |
| `cleanupExpiredRecords()` | Daily auto-delete expired records       |
| **Firebase Scheduler** | Run daily cleanup or scheduled jobs        |



## 🧠 Database (NoSQL)

| Tool              | Purpose                                          |
|-------------------|--------------------------------------------------|
| **Firebase Firestore** | Store user data, lab records, experiments   |
| `users → {uid}`       | User profile document                       |
| `records → {recordId}`| Lab record metadata per subject             |
| `experiments → {expNo}` | Each experiment row per record             |
| **Indexed Fields**   | `createdAt`, `expiryDate` for fast querying   |



## 📦 File Storage

| Tool              | Purpose                                          |
|-------------------|--------------------------------------------------|
| **Firebase Storage** | Store generated PDFs per user                 |
| Path Example       | `/users/{uid}/records/{recordId}.pdf`          |
| Storage Rules      | Auth-based access for secure file control      |



## 📊 Analytics & Tracking

| Tool              | Purpose                                          |
|-------------------|--------------------------------------------------|
| **Google Analytics** | Track usage patterns, logins, PDF generation |
| `gtag()` Events    | Login method, PDF click, QR matched            |



## 📈 Roadmap & Project Management

| Tool              | Purpose                                          |
|-------------------|--------------------------------------------------|
| **GitHub Projects** | Organize features in Kanban/Timeline view     |
| Labels Used        | `frontend`, `backend`, `auth`, `core`, `stretch` |
| `ROADMAP.md`       | Phase-wise checklist and release tracking      |
| `README.md`        | Main documentation with live status            |



## 🗃 Hosting & Deployment

| Tool              | Purpose                                          |
|-------------------|--------------------------------------------------|
| **GitHub Pages**   | Host the frontend static site (HTML/CSS/JS)    |
| **Firebase Console** | Manage backend, DB, auth, and storage        |
| **Vercel (optional)** | Use for Next.js or full SSR frontend        |



## 🛡 Security & Access Control

| Feature             | Purpose                                        |
|---------------------|------------------------------------------------|
| **Firebase Auth**    | Ensures secure access                         |
| **Firestore Rules**  | Limit DB reads/writes to correct users        |
| **Storage Rules**    | Allow each user to access only their PDFs     |
| **Expiry Dates**     | Prevent long-term storage abuse               |



## 💡 Concepts & Practices

| Concept                 | Description                                |
|--------------------------|--------------------------------------------|
| **Serverless Architecture** | Using Firebase for backend with no server |
| **Scalable DB Design**   | Document-subcollection nesting in Firestore |
| **PDF as a Service**     | One-click, QR-enabled lab record export     |
| **Smart Match**          | Suggest GitHub repos based on exp title     |
| **Auto-Cleanup Logic**   | Storage + Firestore cleanup after 40 days   |



## 🔌 Optional / Future Integrations

| Tool / Feature         | Purpose                                      |
|-------------------------|----------------------------------------------|
| **Supabase**            | Alternate DB & auth if migrating from Firebase |
| **Netlify Functions**   | Lightweight backend alternative              |
| **EmailJS / Twilio**    | Send WA/email alerts on generation           |
| **PWA Support**         | Turn KaptureLab into installable app         |
| **Short Link Generator**| Shareable links for records (`kaptu.re/abc`) |

