
# 🍦 Ice Cream Flavors Animation — React + Vite + TailwindCSS

This is a dynamic, visually engaging React project built with Vite, showcasing animated transitions between various ice cream flavors. It utilizes custom animations, TailwindCSS, and image-based interactions to create a delightful user interface.

---

## 🚀 Project Overview

This project demonstrates:
- 🍓 Smooth transition of product names and images with custom animation.
- 🎨 Use of TailwindCSS for styling and utility-first responsiveness.
- ⚛️ React functional components with state-based control.

### 🚀 Live Demo
**[View deployed project here →](https://assignment-gold-six.vercel.app/)**

---

## 📁 Folder Structure

```
root/
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
├── eslint.config.js
├── README.md
├── public/
└── src/
    ├── assets/             # Image files for the ice cream cones
    ├── components/
    │   └── Hero.jsx        # Main animated component
    └── main.jsx            # Entry point
```

---

## ⚙️ Setup & Development

### Prerequisites
- Node.js (v18+ recommended)
- npm or yarn

### 📦 Installation

```bash
# Clone the repository
git clone <repo-url>

# Navigate into the folder
cd <project-folder>

# Install dependencies
npm install
```

### 🔧 Development

```bash
npm run dev
```

This will start the Vite dev server at `http://localhost:5173`.

---

## 🛠️ Technologies Used

- **React 19**
- **Vite**
- **TailwindCSS**
- **Custom CSS animations**

---

## 🚧 Known Issues / Limitations

- Currently no routing implemented (Single Page Static Component).
- Responsiveness may require further refinement for mobile views.
- No unit or integration tests are included.

---

## 📖 Internal Comments & Documentation

- The `Hero.jsx` component manages the flavor image animations and text transitions.
- Animations are controlled via state (`imageAnimating` and `fadeOut`) and trigger based on `index` change.
- Custom `@keyframes` should be added to your CSS (not in Tailwind config) for `comeIn` and `goOut` animations.

**Example (global CSS):**

```css
@keyframes comeIn {
  0% { opacity: 0; transform: translate(50px, 50px) scale(0.9); }
  100% { opacity: 1; transform: translate(0, 0) scale(1); }
}
@keyframes goOut {
  0% { opacity: 1; transform: translate(0, 0) scale(1); }
  100% { opacity: 0; transform: translate(-50px, -50px) scale(0.9); }
}
```

---

## 📄 License

This project is open-sourced for educational and demonstration purposes. Feel free to fork, learn, and enhance.
