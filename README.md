<div align="center">
  <img src="public/assets/icons/logo-full.svg" alt="Janji Sehat Logo" width="200">
    
  **A modern web-based platform that simplifies appointment scheduling between patients and healthcare providers, ensuring a seamless experience for all.**
  
  [![Next.js](https://img.shields.io/badge/Next.js-15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
  [![TailwindCSS](https://img.shields.io/badge/Tailwind%20CSS-v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
  [![Appwrite](https://img.shields.io/badge/Appwrite-F02E65?style=for-the-badge&logo=appwrite&logoColor=white)](https://appwrite.io/)
  [![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=shadcnui&logoColor=white)](https://ui.shadcn.com/)
</div>

<br />

<div align="center">
  <a href="https://janji-sehat.vercel.app">
    <img src="public/assets/images/homepage.png" alt="Janji Sehat App Preview" width="750" style="border-radius: 8px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1); margin-bottom: 24px;">
  </a>
</div>

---

## ⚡ Main Philosophy: Modernizing Healthcare Access
Janji Sehat is intentionally architected to streamline and modernize healthcare services. It bridges the communication gap between patients and medical staff by providing a unified, easy-to-use digital interface.

- **Seamless Scheduling**: Easily book appointments with preferred doctors based on real-time availability.
- **Centralized Health Records**: Users can securely maintain their personal health records and history directly within their profiles.
- **Admin Control**: Robust administrative capabilities to effortlessly manage, approve, or cancel patient appointments.

---

## 🖥️ Application Structure
Janji Sehat is designed with specific workflows to cater to both patients and healthcare administrators.

1. **Patient Portal**
   The core interface for patients to manage their health journey.
   - **Authentication**: Secure login via an OTP passcode sent directly to the user's registered email.
   - **Profile Management**: A dedicated space to detail health history and medical notes.
   - **Appointment Booking**: An intuitive scheduling interface to request new appointments.

2. **Admin Dashboard**
   The centralized command center for administrators (accessible via passkey).
   - **Appointment Management**: View the complete list of requested appointments.
   - **Action Center**: Instantly approve or reject appointment requests, triggering automated email notifications to the respective patients.

---

## ✨ Features
The application is built with modern web technologies focusing on security, speed, and usability.

- **🪪 Secure Passcode Login**: Passwordless authentication system utilizing email-delivered OTPs for patients, and a secure passkey (`123321`) for admins.
- **📅 Dynamic Scheduling**: An intuitive interface for patients to select dates, times, and preferred doctors.
- **🔔 Automated Notifications**: Email alerts to keep patients informed whenever their appointment status changes (e.g., approved or cancelled).
- **🌗 Premium Aesthetics**: A beautifully crafted UI using `shadcn/ui` and Tailwind CSS, providing a clean, accessible, and premium user experience.

---

## 🛠️ Built With

| Tech Stack | Purpose |
| :--- | :--- |
| **Next.js** | Core React framework providing App Router and server actions. |
| **TypeScript** | Static typing for complete type safety and robust code architecture. |
| **Tailwind CSS** | Utility-first CSS framework for rapid and consistent UI styling. |
| **Appwrite** | Backend-as-a-Service powering database, authentication, and storage. |
| **shadcn/ui** | Accessible, beautifully designed React components. |
| **SendGrid / Nodemailer** | Email delivery services for OTPs and appointment notifications. |

---

## 🚀 Getting Started

### Prerequisites
Make sure you have **Node.js** and **npm** installed on your system.

### 1. Clone the Repository
```bash
git clone https://github.com/yossyadirta/janji-sehat.git
cd janji-sehat
```

### 2. Install Dependencies
```bash
npm install
# or
yarn install
```

### 3. Set Environment Variables
Create a `.env.local` file in the root directory and configure it based on your Appwrite and Email provider setup:

```env
NEXT_PUBLIC_API_URL=your_api_url
NEXT_PUBLIC_SENDGRID_API_KEY=your_sendgrid_api_key
NEXT_PUBLIC_APPWRITE_PROJECT_ID=your_appwrite_project_id
NEXT_PUBLIC_APPWRITE_ENDPOINT=your_appwrite_endpoint
NEXT_PUBLIC_ADMIN_PASSCODE=123321

NEXT_PUBLIC_PROJECT_ID=your_public_project_id
NEXT_PUBLIC_API_KEY=your_api_key
DATABASE_ID=your_database_id
PATIENT_COLLECTION_ID=your_patient_collection_id
DOCTOR_COLLECTION_ID=your_doctor_collection_id
APPOINTMENT_COLLECTION_ID=your_appointment_collection_id
AUTH_SESSION_COLLECTION_ID=your_auth_session_id
NEXT_PUBLIC_BUCKET_ID=your_bucket_id
NEXT_PUBLIC_ENDPOINT=your_appwrite_endpoint
NEXT_PUBLIC_ADMIN_PASSKEY=your_admin_passkey
```

### 4. Run the Development Server
```bash
npm run dev
# or
yarn dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.
