# NEUScan | NEU Library Visitor App

NEUScan is a real-time visitor management and analytics platform designed specifically for New Era University Library. The platform digitizes student entry via institutional e-mails and QR codes, while providing administrators with deep insights into library usage patterns.

________________________________________

## ✨ Production Features

Designed as a context-aware HUD with a dynamic design, the header ensures users stay informed and engaged with library operations. 

### 🔹 For Students and Faculty
• **Smart QR Entry**: A single, persistent QR code for both entrance and exit for instant identity verification. The system automatically toggles status based on last scan. 
• **Visit Registration**: A digital form to select "Reason for Visit,” replacing manual logbooks and enabling admins to gain meaningful insights into library usage and student needs.
• **Instant Success Feedback**: Upon submission, students are redirected to a dedicated "Welcome to NEU Library!" success page.
• **Live Announcement Board**: Real-time updates on library operations and events. 
• **Feedback System**: Directly share experiences and suggestions with library administration through a dedicated portal.

### 🔹 For Admin 
• **Live Occupancy Monitoring**: Real-time tracking of the current library population across different zones, with data organized by daily, monthly, and yearly trends.
• **Automated Data Logging**: Instant Firestore documentation of all visits, reasons for entry, and exit timestamps. 
• **Announcement Management**: Broadcast urgent notices and manage the public Announcement Board seen by students.
• **System Controls**: Manual and automated overrides for library operating status (Open/Closing/Closed).

________________________________________

## 🛠️ Tech Stack
• **Framework**: Next.js 15 (App Router)
• **Frontend**: React 19, Tailwind CSS
• **UI Components**: ShadCN UI (using Radix UI primitives)
• **Animations**: Framer Motion for smooth page transitions
• **Database & Auth**: Firebase (Firestore & Authentication)
• **Charts**: Recharts for data visualization
• **Communication**: Real-time listeners via Firestore `onSnapshot`

________________________________________

## 📝 Demo Instructions (Reviewers Only)

> [!IMPORTANT]
> **Demo Access for Testing**
> Since admin access cannot be granted automatically via Google account sign-in, a Demo Access feature has been implemented. This allows you to:
> • Test as an administrator without needing a Google account.
> • Simulate student or faculty access for testing purposes.

### Steps to Use Demo Access
1. **Launch the application.**
2. **Select a role on the login screen** by clicking either the “Student/Faculty” or “Admin” button located below the Demo Access option.

#### a. Student/Faculty:
• You will be automatically logged in as a demo student:
  - **Name**: Juan Dela Cruz
  - **Email**: demojuan.delacruz@neu.edu.ph
• Simulate a check-in by selecting a “Reason for Visit” and pressing the “Demo: Simulate Scan” button.
• You will then be directed to the “Welcome to Library!” success page. Press “Demo: Simulate Exit” to sign out.

#### b. Admin:
• You will gain access to all admin controls, including:
  - Real-time activity monitoring
  - Visitor analytics
  - Zone analytics
  - Student satisfaction tracking
  - Library status control
  - Announcement management

________________________________________

## 🛡️ Safety & Security
• **30-Second Cooldown**: Prevents accidental double-scans from toggling a user out immediately.

________________________________________

## 📂 Project Structure
• **src/app**: Next.js 15 App Router pages, layouts, and API routes.
• **src/components**: Reusable ShadCN components and specialized dashboard widgets.
• **src/firebase**: Configuration, specialized hooks (useCollection, useDoc), and data mutation utilities.
• **src/lib**: Core utility functions, logic for "Reason for Visit" categorization, and TypeScript definitions.

________________________________________

## 📜 License
This project is developed for the New Era University Library, as part of academic requirements. All rights reserved.
