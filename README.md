# 🔐 Encrypted File Vault 🛡️

## Secure & Scalable MERN Stack File Management System

[![GitHub last commit](https://img.shields.io/github/last-commit/Git-brintsi20/1.CyberProj_Mern_Auth_Sys?color=blue&style=for-the-badge)](https://github.com/Git-brintsi20/1.CyberProj_Mern_Auth_Sys/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

---

### ✨ Overview

The **Encrypted File Vault** is a robust, full-stack MERN (MongoDB, Express.js, React, Node.js) application designed for highly secure personal or organizational file management. It prioritizes data privacy and integrity by implementing advanced cryptographic techniques and comprehensive security measures.

**Key Highlight:** This project demonstrates a deep understanding of full-stack development, modern frontend frameworks (React with Shadcn UI/TailwindCSS), and, most importantly, **critical backend security practices and cryptographic implementations** crucial for protecting sensitive user data.

---

### 🚀 Live Demo (Optional - Add your Render/Vercel URL here if deployed)

**[🔗 Access the Live Encrypted File Vault Here!](YOUR_RENDER_FRONTEND_URL_HERE)**
*(Please note: Free tier deployments might experience cold starts.)*

---

### 🎥 Sneak Peek (Optional - Add your GIF/Screenshot here)

*(Consider adding a short GIF or a compelling screenshot demonstrating the UI, especially the drag-and-drop, dashboard, and 2FA setup.)*

![Project Screenshot/GIF Placeholder](assets/screenshot-placeholder.gif)

---

### 🌟 Core Features & Technologies

#### Frontend Experience (React, Vite, Shadcn UI, TailwindCSS)
* **Intuitive Drag-and-Drop Uploads:** Seamless file uploads with smooth animations and clear progress indicators.
* **Dynamic File Management Dashboard:** Modern grid/list view toggle for easy navigation and management of encrypted files.
* **Interactive Progress Bars:** Real-time upload/download progress with fluid animations.
* **Secure Authentication Interfaces:** Dedicated interfaces for 2FA setup (QR code generation) and Email OTP verification.
* **Safe File Preview:** In-browser preview capabilities for secure file types (e.g., images, PDFs) after decryption.
* **Elegant Modals:** Smooth modal animations for all file operations (delete, share, preview).

#### Backend Security (Node.js, Express.js, MongoDB)
* **File Encryption (AES-256-GCM):** Industry-standard symmetric encryption for all uploaded files.
    * **Why AES-256-GCM?** Chosen for its robust encryption (256-bit key length) combined with **Authenticated Encryption with Associated Data (AEAD)**. GCM mode provides crucial **integrity checking** and **authenticity verification** via an authentication tag, preventing sophisticated tampering attacks.
* **Unique Encryption Keys per User:** Each user's files are encrypted with keys derived uniquely for them, enhancing isolation.
* **2FA Implementation (TOTP with `speakeasy`):** Time-based One-Time Passwords for an extra layer of login security.
* **Email OTP Verification (`nodemailer`):** Secondary verification via email for critical actions or login.
* **Secure File Storage:** Encrypted files stored in a non-web-accessible directory with unique, unguessable filenames (UUIDs).
* **Metadata Encryption:** Sensitive file metadata (IVs, Auth Tags, checksums) are securely stored alongside the encrypted content.
* **File Integrity Verification:** Checksums (SHA256) are generated on original files and verified upon download to detect any unauthorized modifications.
* **Secure Key Derivation (PBKDF2):** Passwords are never stored directly; strong, user-specific encryption keys are derived using PBKDF2, resisting brute-force and rainbow table attacks.

#### Comprehensive Security Implementations
* **Client-Side File Type Validation:** Initial validation for common file types.
* **Server-Side File Scanning (Conceptual):** Architecture supports integration with external virus scanning services.
* **Rate Limiting:** Prevents brute-force attacks on authentication endpoints and abuse of upload/download features.
* **User Activity Logging:** Detailed audit trail for significant user actions (logins, uploads, downloads, shares).
* **Session Timeout Management:** JWT-based session management with configurable expiry.
* **Password Strength Enforcement:** Ensures users create strong, complex passwords during registration.

#### Advanced Capabilities
* **File Sharing with Temporary Links:** Securely share files via time-limited, one-time-use links.
* **Audit Trail for File Access:** Comprehensive logging provides visibility into all file operations.
* **File Versioning:** Maintain encrypted historical versions of files.
* **Recovery Key Generation (Conceptual):** Supports the creation of recovery keys for account access.

---

### 🛠️ Technologies Used

**Frontend:**
* **React:** Frontend library for building user interfaces.
* **Vite:** Fast development server and build tool.
* **TypeScript:** Type-safe JavaScript.
* **Shadcn UI & Radix UI:** Beautiful, accessible, and customizable UI components.
* **Tailwind CSS:** Utility-first CSS framework for rapid styling.
* **`@tanstack/react-query`:** Powerful data fetching and caching for API interactions.
* **`react-router-dom`:** Declarative routing for React.
* **`react-hook-form` & `zod`:** Robust form validation.
* `input-otp`, `sonner`, `lucide-react`, etc.

**Backend:**
* **Node.js & Express.js:** Backend runtime and web framework for RESTful APIs.
* **MongoDB & Mongoose:** NoSQL database and ODM for data storage.
* **`bcryptjs`:** Password hashing.
* **`jsonwebtoken`:** JWT for authentication.
* **`multer`:** Handling file uploads.
* **`crypto` (Node.js built-in):** AES-256-GCM encryption, SHA256 hashing.
* **`speakeasy` & `qrcode`:** For 2FA implementation.
* **`nodemailer`:** Email sending for OTPs.
* **`express-rate-limit`:** Middleware for rate limiting.
* **`dotenv`:** Environment variable management.

---

