1 file changed
+34
-5
GITHUB_PROFILE_README.md
# Hi, I'm Robin Singh 👋

### Backend Developer | Building secure, scalable web systems with JavaScript
### JavaScript Developer | Building secure, scalable full-stack web experiences

I enjoy turning product ideas into reliable backend services—especially where authentication, cloud storage, and clean API design meet. I am currently focused on strengthening my Node.js ecosystem skills and building projects that solve practical problems.
I enjoy turning product ideas into reliable web experiences—especially where a smooth client experience meets secure APIs, cloud storage, and clean data design. I am currently focused on strengthening my JavaScript and Node.js ecosystem skills by building practical, end-to-end products.

## What I Work With

<p>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/REST_API-005571?style=for-the-badge" alt="REST API" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/AWS_S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white" alt="AWS S3" />

## Featured Project

### [Loader — Secure File Management API](https://github.com/robin1117/Express-File-Sharing-Server-System-)
### [Loader — Secure File Management System](https://github.com/robin1117/Express-File-Sharing-Server-System-)

A production-minded REST API that enables users to manage cloud-hosted files and folders securely.
A full-stack-ready file management system designed around a browser client and a secure REST backend. Users can register, sign in, create folders, upload files, browse their storage, preview/download content, and manage sessions.

### End-to-End Flow

```text
Browser / Frontend
  │  CORS-enabled REST requests + signed session cookie
  ▼
Express.js API
  ├── Authentication & authorisation ──► Redis sessions
  ├── User, folder & file metadata ────► MongoDB / Mongoose
  ├── File uploads & secure access ────► AWS S3
  └── OTP and reset emails ────────────► Resend
```

### Frontend ↔ Backend Integration

| User experience | Backend capability |
| --- | --- |
| Sign up and sign in | Validation, bcrypt password hashing, signed HTTP-only cookie sessions |
| Google / GitHub login | OAuth code exchange and account creation |
| File browser | Directory listing API returns folders, files, and breadcrumbs |
| Upload progress / resume | S3 multipart upload endpoints with chunk offsets and resume checks |
| File preview or download | Short-lived S3 pre-signed URL redirect |
| Password recovery | Email OTP and one-time reset-token workflow |
| Account/session controls | Current-session logout, logout from all devices, role-aware controls |

### Engineering Highlights

- Built authentication with **bcrypt**, signed HTTP-only cookies, and **Redis-backed sessions**.
- Added **Google** and **GitHub OAuth**, email OTP verification, and password-reset flows.
- Implemented folder creation, browsing, renaming, and recursive deletion with **MongoDB/Mongoose**.
- Designed **AWS S3 multipart and resumable uploads**, plus short-lived pre-signed URLs for private file access.
- Enabled browser-client integration through configurable **CORS**, JSON APIs, cookies, and upload response headers.
- Used **Zod** for request validation and MongoDB transactions for reliable account setup.

**Stack:** Node.js · Express · MongoDB · Mongoose · Redis · AWS S3 · OAuth 2.0 · Zod · Resend
**Backend stack:** Node.js · Express · REST APIs · MongoDB · Mongoose · Redis · AWS S3 · OAuth 2.0 · Zod · Resend

## Currently Learning

