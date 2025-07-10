# 🧩 KaptureLab – Dev Portions (Engineer Roles)

> A full-stack solo-dev breakdown of the KaptureLab project.  
> Switch between portions based on your interest or energy level.

---

## 🎨 Portion 1: Frontend Development (UI/UX)

**Role**: UI Engineer  
**Goal**: Design the full user interface and user interactions

### ✅ Tasks:
- [ ] Login page with Google/GitHub/Guest
- [ ] Lab record form (subject, reg. no., rows)
- [ ] Dynamic add/remove experiment rows
- [ ] Responsive layout for desktop
- [ ] PDF preview section
- [ ] Buttons: Generate, Download, Reset
- [ ] Alerts and validation messages

---

## 🔐 Portion 2: Authentication (Auth & Session)

**Role**: Identity Engineer  
**Goal**: Handle all login and user identification logic

### ✅ Tasks:
- [ ] Setup Firebase Project
- [ ] Enable Google login
- [ ] Integrate GitHub OAuth login
- [ ] Handle Guest login with localStorage
- [ ] Save user info in Firestore
- [ ] Protect pages using auth state

---

## ☁️ Portion 3: Backend + Database (Firestore + Storage)

**Role**: Backend Engineer  
**Goal**: Save and retrieve user-generated data securely

### ✅ Tasks:
- [ ] Firestore structure: users → records → experiments
- [ ] Save record metadata (subject, createdAt, expiryDate)
- [ ] Upload PDFs to Firebase Storage (path: /users/{uid}/records/)
- [ ] Save PDF link in Firestore
- [ ] Add Firestore & Storage security rules

---

## 📄 Portion 4: PDF & QR Generator

**Role**: Document Engineer  
**Goal**: Generate smart PDF lab records

### ✅ Tasks:
- [ ] Integrate html2pdf.js
- [ ] Generate QR codes from GitHub links
- [ ] Build clean lab template layout
- [ ] Show live preview before download
- [ ] Upload PDF after generation

---

## 🔁 Portion 5: GitHub Repo Match Logic

**Role**: API Engineer  
**Goal**: Make the platform smart with GitHub integration

### ✅ Tasks:
- [ ] GitHub OAuth token exchange (via Firebase Function)
- [ ] Fetch user repos from GitHub API
- [ ] Auto-suggest repo names in form
- [ ] Insert matched repo link into row
- [ ] Generate QR from link

---

## 🧹 Portion 6: Auto Cleanup System

**Role**: Systems Engineer  
**Goal**: Automate storage cleanup after 40 days

### ✅ Tasks:
- [ ] Save createdAt and expiryDate in Firestore
- [ ] Firebase scheduled function to check expiry
- [ ] Delete PDFs from Firebase Storage
- [ ] Delete Firestore metadata

---

## 📊 Portion 7: Analytics + Polish

**Role**: Growth Engineer  
**Goal**: Final experience refinement + insights

### ✅ Tasks:
- [ ] Add Google Analytics script
- [ ] Track login, repo match, PDF generation
- [ ] UI polish and feedback messages
- [ ] “Project Cooked” message
- [ ] Deploy on GitHub Pages

---

## 🧠 Summary Table

| Portion | Role You’re Playing | What You’re Building          |
|---------|----------------------|-------------------------------|
| 1       | UI Engineer          | Frontend layout, interactions |
| 2       | Auth Dev             | Google/GitHub login           |
| 3       | DB Engineer          | Firestore & Storage handling  |
| 4       | Doc Engineer         | PDF & QR export               |
| 5       | API Integrator       | GitHub repo autofill          |
| 6       | Systems/DevOps       | Auto-cleanup logic            |
| 7       | Growth Engineer      | Analytics + polish            |

---

🛠 **Work smart. Switch portions when bored.  
Own every part like a solo team. Deliver like a SaaS engineer.**
