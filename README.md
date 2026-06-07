# 🛡️ Reflect — AI Skill Verification & Resume Builder

Reflect is a state-of-the-art web application that allows candidates to build professional resumes and back them up with cryptographic, proctored, and AI-verified skill assessments. 

## 🌐 Live URL
👉 **[https://reflect-ai-resume.vercel.app](https://reflect-ai-resume.vercel.app)**

---

## ✨ Key Features

1. **🔐 Multi-Channel Authentication**:
   - **Email & Password**: Standard credential registration.
   - **Google Sign-In Simulation**: Features a mockup of the Google Account Chooser and Permissions Consent popup.
   - **Phone & OTP**: 6-digit OTP verification flow.

2. **⚡ Speed Evaluation Mode**:
   - Skip manual data entry! Click "Load Google Sample Profile" on onboarding to instantly populate a completed, top-tier Google Software Engineer profile with verified test scores, proctoring statistics, and hidden talents.

3. **🎨 16 Premium Resume Templates**:
   - A range of options from Trending Gradients and Creative Sidebars to Technical developer formats and a customized Google Material Design template.

4. **👁️ Biometric Identity Verification**:
   - Fully client-side liveness detection challenges (e.g., look straight, blink, smile, head turns) using MediaPipe's Face Landmark models. Includes a graceful bypass option if cameras or detection fail.

5. **🔍 Proctored Skill Assessment**:
   - High-fidelity exam interface with automated anti-cheat systems:
     - Tab-switch monitoring (warning triggers).
     - Copy-paste prevention.
     - Eye-tracking proctoring via a persistent floating web camera.
   - Pre-loaded with easy-to-medium real questions for 20+ major skills.

6. **📊 Analytics Dashboard**:
   - Gorgeous data visualizations (Radar charts, Bar charts, Doughnut metrics) representing skill matrix, accuracy breakdown, and profile strength.

7. **📥 Premium Exports (PDF, PNG, DOCX)**:
   - Export both the **Resume** and the **Official Skill Analytics Report**!
   - Supports high-resolution PDF and PNG downloads.
   - Supports Microsoft Word (**DOCX**) format. Chart.js canvases and QR code SVGs are dynamically converted to base64 images and embedded inline, keeping layout, charts, and styling intact in Word.

8. **🔗 Verification QR Code**:
   - Each export embeds a verification QR code and a cryptographic hash for employers to check candidates' authenticity logs.

---

## 🛠️ Technology Stack

* **Frontend**: React 18 (Vite-powered Single Page App)
* **Routing**: React Router v6
* **Styling**: Vanilla CSS (CSS variables, glassmorphism, responsive grid)
* **Graphics**: Chart.js + react-chartjs-2
* **Computer Vision**: @mediapipe/tasks-vision
* **Export Utilities**: html2canvas + jsPDF
* **QR Codes**: react-qr-code

---

## 🚀 Local Setup

To run this project on your machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone <your-github-repo-link>
   cd Refiect
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm run dev
   ```

4. **Build for production**:
   ```bash
   npm run build
   ```

---

## ☁️ Deploying to Vercel

Reflect is configured for easy deployment on **Vercel** with single-page app routing overrides.

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Deploy**:
   Run the following command in the project root:
   ```bash
   vercel --prod
   ```
   Follow the prompts to deploy the website instantly.
