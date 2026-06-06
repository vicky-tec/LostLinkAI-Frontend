# LostLink AI — Frontend UI Client

A premium, state-of-the-art visual client for **LostLink AI**, an AI-powered lost-and-found recovery system built for college campuses. This client leverages modern design aesthetics, accessibility, and clean micro-interactions to deliver a frictionless experience for students, faculty, and campus administrators.

---

## 🎨 Design & Visual System
- **Rich Aesthetics:** Designed with custom Glassmorphism, deep dark AI theme, sleek light mode, and high-contrast accessibility tags.
- **Floating Dual Navigation:**
  - **Desktop:** Floating navigation bar with blur effect.
  - **Mobile:** Bottom capsule tab bar configured for quick thumb access.
- **8px Layout Grid:** Strict spacing consistency across all pages.
- **Holographic Scans:** Found Item report includes a simulated laser scanning animation representing Gemini visual processing.

---

## ⚡ Main Pages & Features

### 1. Hero Landing Page
- Interactive Bento metrics showing live stats.
- Bhagavad Gita quote of the day.
- Match concept radar showing interactive matching.

### 2. Holographic Upload (`/report-found`)
- Large drag-and-drop zone with shimmering upload states.
- Live progress logger showing step-by-step API processing.
- Gemini Verification Certificate containing detected parameters.

### 3. Missing Report (`/report-lost`)
- Multi-field input grid for registering lost items.
- Inline recommendation widget showing potential matches from the database immediately.

### 4. AI Match Engine (`/matches`)
- Comparative dual-pane workspace.
- Cosine similarity circles (SVG indicators).
- Gemini rationale text and document OCR logs.

### 5. Claims Validation (`/claims`)
- Ownership proof verification.
- Staged timeline tracker (Submitted → Under Review → Approved/Completed).

---

## 🛠️ Technology Stack
- **Framework:** React + Vite
- **Styling:** TailwindCSS + Vanilla CSS Variables
- **Icons:** Lucide React + Material Symbols
- **State/Routing:** React Router DOM
- **Utility:** date-fns, react-hot-toast

---

## 🚀 Local Setup Instructions

1. **Install Dependencies:**
   ```bash
   npm install
   ```

2. **Configure API Endpoints:**
   Open `src/api.js` and configure the `baseURL`:
   - For local development: `'/api'` (uses the Vite proxy target configured in `vite.config.js`).
   - For production: `'https://your-backend-vercel-url.vercel.app/api'`.

3. **Start Development Server:**
   ```bash
   npm run dev
   ```
   Open `http://localhost:5173` in your browser.

4. **Production Build:**
   ```bash
   npm run build
   ```
