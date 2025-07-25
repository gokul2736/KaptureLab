<h1 align="center"> KaptureLab</h1>

<p align="center">A simple tool to generate clean, QR-enabled lab record PDFs — right from your browser.</p>


<h2 align="center"> What is KaptureLab?</h2>
<p align="center">KaptureLab is a smart lab record PDF generator platform for students that allows you to generate QR-linked PDFs, 
auto-fill GitHub experiment links, and securely store your documents — all with ease.</p>

## 🛠️ Project Status: Currently Cooking... 🍳

KaptureLab is in **active development** — we're still baking the core features.

Major updates are being pushed regularly do expect improvements in:  
- Design and UI flow  
- GitHub OAuth integration  
- PDF + QR generation  
- Firestore & Storage logic  

This README, the tech stack, and the roadmap will evolve as the project gets closer to completion.  
**Stay tuned and watch the repo ⭐ if you're interested!**

##  Features (Planned & In Progress)

- 🔐 Login via Google, GitHub, or Guest mode
- 📄 Dynamic form for lab records
- 🔗 Smart auto-match GitHub repos per experiment
- 🧾 Generate clean, college-style PDF with QR
- ☁️ Upload to Firebase Storage
- ⏳ Auto-delete after 40 days
- 📊 Google Analytics for tracking usage
- 💬 Dashboard view for all records (coming soon)

## Tech Stack

 Do Check [`TECH STACK.md`](https://github.com/gokul2736/KaptureLab/blob/main/TechStack.md) 

## 🧾 License

This project is licensed under the **Creative Commons BY-NC 4.0** license.
CC BY-NC 4.0 — Free for personal/student use. No commercial redistribution.
Read more: [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

##  Contribution

Have an idea? Found a bug?  
Open an issue or make a pull request!



### 📄 Lab Record Form
- Dynamic row addition for each experiment
- **Auto-numbering** for experiment numbers
- Date selection via calendar input
- Title input with **GitHub repo suggestion dropdown**
- Repo auto-linking logic via partial match


## 🚀 Tech Used

- **Frontend:** ReactJS + JavaScript (SPA, component-based)
- **PDF Generator:** `jsPDF`, `html2canvas`, `qrcode.react`
- **Backend:** Firebase Auth, Firestore DB, Firebase Storage
- **GitHub API:** OAuth & public repo fetching

## ✅ Status: Actively Developing

- Frontend React setup ✅  
- Auth flow (Google/GitHub) ✅  
- Form structure and PDF generation ⏳  
- GitHub repo suggestion logic ⏳  
- Auto-delete and cloud storage ⏳  
- Dashboard with record viewer ⏳

> Last updated: **July 2025** | Maintained by: [Gokul](https://github.com/gokul2736)
