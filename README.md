# 🧩 Sample WordPress Plugin – PHP & VueJS

This repository is a custom WordPress plugin built to demonstrate how I adapt my React expertise into other
frameworks like Vue while maintaining a high standard of quality.

It showcases production‑ready code with clean UI interactions, real‑time data handling, and adherence to WordPress best practices.

Originally, it was developed for a coding challenge but it has since been refined into a professional example for recruiters and
engineering teams to review my coding skills and front‑end capabilities.

---

## 📦 What is this project?

This is a **WordPress plugin** with a simple design and a modern front-end stack to showcase:

- ⚙️ Vue.js integration with WordPress admin
- 🔌 Custom WordPress REST API endpoints
- 🔐 Secure data handling following WordPress best practices
- 🎨 Custom UI components built with accessibility in mind
- 📦 A complete plugin packaging workflow (Composer + NPM)

The plugin provides an admin interface where data is fetched via custom REST routes and displayed dynamically through Vue components.

---

## 🧑‍💻 Key Technical Highlights

- 💼 **Role**: Sole developer (WordPress + Vue)
- 🏗️ **Architecture**: Vuex store for state management connected to WordPress REST routes
- 🔄 **Real-time Updates**: Axios-driven calls with graceful loading states
- 📐 **Accessibility**: ARIA attributes for feedback messages
- 📚 **Testing**: Ready-to-run Jest tests
- 🔧 **Build Process**: NPM + Webpack for scripts/styles, Composer for PHP dependencies

---

## 🚀 Getting Started

### Prerequisites

- Node.js v18.16.0 or later
- Composer v2+
- WordPress 6.0+

### Installation

Clone or download the plugin into your WordPress plugins folder:

```bash
cd <path-to-wordpress>/wp-content/plugins
git clone https://github.com/<your-repo>/leighton-quito
```

Install Node dependencies:

```bash
npm install --legacy-peer-deps
```

Install PHP dependencies:

```bash
composer install
```

### WordPress Environment

Before **activating** the plugin, ensure you set your permalinks to **post name**, for that:

On the WordPress dashboard, go to Settings → Permalinks Screen. Choose "Post name" as you permalink structure, and click on "Save changes" button.

---

## 🛠️ Development Scripts

- `npm run dev` – Run Webpack in watch mode for scripts and styles.
- `npm run tokens` – Build design tokens into `./assets/scss/_utils/_tokens.scss`.
- `npm run test` – Run the unit tests.

---

## 📦 Production Scripts

- `npm run prod` – Compile assets for production.
- `npm run release` – Prepares a full release:
  - Build tokens
  - Compile assets
  - Generate translations
  - Copy files into a `dist/` folder
  - Package as a versioned `.zip` ready for distribution

---

## ✅ Submission Criteria Alignment

| Requirement              | How it's Met                                                                 |
|--------------------------|------------------------------------------------------------------------------|
| **Semantic HTML**        | Vue components use semantic markup with proper ARIA roles.                   |
| **Custom CSS/UI**        | Styles are built from scratch; no frameworks used.                           |
| **Component Architecture** | Vuex store and modular Vue components.                                       |
| **No jQuery**            | All JavaScript uses modern ESNext and Vue.                                   |
| **Accessibility**        | Success messages and buttons include ARIA attributes for screen readers.      |
| **WordPress Integration**| Uses `wp_localize_script`, `rest_api_init`, and secure permission callbacks.  |

---

## 📂 Explore the Code

- `assets/` – Vue.js app, Vuex store, and compiled styles/scripts
- `includes/` – Custom PHP classes for REST API routes
- `Api.php`, `Data_Route.php` – WordPress REST route definitions
- `DataPreview.vue` – Vue component rendering dynamic data
- `Admin.php` – Registers scripts and initializes plugin admin

---

If you'd like to dive deeper into any piece, I'd be happy to walk you through it.

— **Leighton Quito**
