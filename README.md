# StoreIt

Store-It SM is a modern **file storage and management web application** built with **Next.js**, **React**, **TailwindCSS**, and **Appwrite**. This project was created following a **JavaScript Mastery YouTube tutorial**.

Key highlights:

* **Secure email OTP authentication** using Appwrite
* **Complete file management**: upload, rename, delete, and share files with other users
* **Real-time search and filtering** with debounced inputs for optimal performance
* **Dashboard with visual file usage analytics** powered by Recharts
* **Dynamic thumbnail previews** for images, videos, and documents
* Fully **responsive UI** built with Radix UI components and TailwindCSS

---

## 📖 Pages

### 🔐 User Authentication

* Email OTP verification system via Appwrite
* Secure session management and user authentication

<img width="769" height="631" alt="storeit1" src="https://github.com/user-attachments/assets/3330664a-5873-45b8-bcd5-514d8c555c88" />

<img width="775" height="627" alt="storeit8" src="https://github.com/user-attachments/assets/3b1683a2-26de-4ed0-ba5c-fb730a30cf72" />

<img width="775" height="625" alt="storeit2" src="https://github.com/user-attachments/assets/60a04d4c-d121-4e1c-8e3a-24b9a87bb605" />

### 📊 Dashboard & Analytics

* **File usage summary** with visual charts
* **Storage statistics** organized by file type
* **Recharts integration** for data visualization

<img width="779" height="601" alt="storeit" src="https://github.com/user-attachments/assets/c93d5e88-6460-490d-89ae-d947c8d21622" />

### 📤 File Management

* **Upload** files directly to Appwrite storage
* **Rename** and **delete** files with confirmation dialogs
* **Share files** with other users via email
* Dynamic thumbnail previews for all file types

<img width="773" height="625" alt="storeit3" src="https://github.com/user-attachments/assets/3c6ed0d2-93ea-452d-b298-92f789711756" />

<img width="771" height="627" alt="storeit4" src="https://github.com/user-attachments/assets/da1bdbbc-3532-449c-8ca2-b87a4b265c5c" />

<img width="771" height="627" alt="storeit5" src="https://github.com/user-attachments/assets/e438c604-d5f7-4bbb-91ab-0d4490326c00" />

---

## 🧩 Features

### 🔍 Search & Filter

* **Real-time file search** with thumbnail results
* **Debounced search** for improved performance
* **Sort files** by creation date, size, name, and more


### 🎨 Responsive Design

* Modern UI built with **Radix UI** components
* **TailwindCSS** styling with custom animations
* Fully responsive across all device sizes

---

## 🛠️ Tech Stack

* **Frontend:** Next.js 15, React 19, TypeScript 5, TailwindCSS 3
* **Backend & Storage:** Node-Appwrite 15 (authentication, database, storage)
* **UI Components:** Radix UI (AlertDialog, Select, Toast, Dropdown Menu)
* **Forms & Validation:** React Hook Form, Zod
* **Charts:** Recharts
* **Utilities:** use-debounce, tailwindcss-animate, clsx, tailwind-merge

---

## ⚡ Installation

### 1. Clone the repository

```bash
git clone https://github.com/SALVADORPOETA/StoreIt-sm.git
cd StoreIt-sm
```

### 2. Install dependencies

```bash
npm install
```

### 3. Setup environment variables

Create a `.env.local` file in the root directory with the following variables:

```env
NEXT_PUBLIC_APPWRITE_ENDPOINT=your-appwrite-endpoint
NEXT_PUBLIC_APPWRITE_PROJECT=your-appwrite-project-id
NEXT_PUBLIC_APPWRITE_DATABASE=your-database-id
NEXT_PUBLIC_APPWRITE_USERS_COLLECTION=your-users-collection-id
NEXT_PUBLIC_APPWRITE_FILES_COLLECTION=your-files-collection-id
NEXT_PUBLIC_APPWRITE_BUCKET=your-bucket-id
NEXT_APPWRITE_KEY=your-secret-key
```

### 4. Run the development server

```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) to view the application.

---

## 🎨 Usage

* **Sign up or sign in** with your email using OTP verification
* **Upload files** directly to Appwrite storage
* **Rename, delete, and share** files with other users via email
* **View your storage summary** in the dashboard with visual analytics
* **Search and filter** files in real-time for easy access
* **Sort files** by creation date, size, name, or type

---

## 📦 Project Structure

```
store-it-sm/
 ├─ app/                       # Next.js app directory
 │  ├─ (auth)/                 # Authentication-related pages
 │  │  ├─ sign-in/
 │  │  │  └─ page.tsx          # Sign-in page
 │  │  └─ sign-up/
 │  │     └─ page.tsx          # Sign-up page
 │  └─ (root)/                 # Root layout and pages
 │     └─ layout.tsx           # Main app layout
 ├─ lib/                       # Utility functions and Appwrite actions
 │  ├─ actions/                # Actions for interacting with Appwrite
 │  │  ├─ file.actions.ts      # File-related actions (upload, delete, fetch)
 │  │  └─ user.actions.ts      # User-related actions (auth, OTP, session)
 │  ├─ appwrite/               # Appwrite configuration
 │  │  └─ config.ts            # Appwrite environment and config
 │  └─ utils.ts                # Helper functions (date, file size, thumbnails, etc.)
```

---

## 📊 Supported File Types

### 📄 Documents
* PDF, DOCX, TXT, XLSX, CSV, and more

### 🖼️ Images
* JPG, PNG, GIF, SVG, WEBP

### 🎥 Videos
* MP4, AVI, MOV, MKV

### 🎵 Audio
* MP3, WAV, FLAC

### 📦 Others
* Any unsupported file types with generic icons

Each file type has a **dynamic thumbnail icon** for better visualization and user experience.

---

## 🔧 Key UI Components

* **OTP Modal** – Email verification with 6-digit code input
* **Search Component** – Real-time file search with thumbnail previews
* **Sidebar** – Navigation menu with user information
* **Sort Dropdown** – Sort files by various criteria
* **Thumbnail Component** – Dynamic previews for all file types
* **File Actions** – Rename, delete, share, and download options

---

## 🌐 Links

* **GitHub:** [https://github.com/SALVADORPOETA/StoreIt-sm](https://github.com/SALVADORPOETA/StoreIt-sm)
* **LinkedIn:** [https://www.linkedin.com/in/salvador-martinez-sm/](https://www.linkedin.com/in/salvador-martinez-sm/)

---

## ⚖️ License

This is a personal portfolio project by Salvador Martinez based on a JavaScript Mastery tutorial. No commercial use intended.
