# 🧩 Contributing to Cab Booking Website

Welcome, and thank you for considering contributing to this open-source **cab booking website project**! 🚖  
This is a **static, frontend-only** project built using **HTML, CSS, JavaScript (ES Modules)**, and **GSAP** for animations. We care about performance, clean code, and creating a welcoming environment for developers of all levels.

---

## 📦 Tech Stack

- HTML5 (Semantic, Accessible)
- CSS3 (Responsive layout, BEM)
- JavaScript (ES6+ modules)
- GSAP (GreenSock Animation Platform)
- No backend or database (static only)
- License: **Apache-2.0**

---

## 🔧 Project Structure

📂 project-root/
│
├── 📁 assets/ → Images, icons, fonts
├── 📁 css/ → Modular stylesheets (can include main.css, variables.css, etc.)
├── 📁 js/ → Modular JavaScript (ES modules)
├── 📁 animations/ → GSAP animation files
├── 📁 components/ → Reusable HTML components (optional for includes or JS templates)
├── 📁 pages/ → Page-specific HTML files
│
├── 📄 index.html → Main landing page
├── 📄 .eslintrc.json → ESLint configuration
├── 📄 .prettierrc → Prettier config for formatting
├── 📄 README.md → Project overview
├── 📄 LICENSE → Apache-2.0 license
└── 📄 CODE_OF_CONDUCT.md → Community behavior guidelines

yaml
Copy
Edit

---

## 👣 Getting Started

1. **Fork** the repository.
2. **Clone** it locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/cab-booking-site.git
   cd cab-booking-site
Create a feature branch:

bash
Copy
Edit
git checkout -b feature/your-feature-name
Make your changes following the conventions below.

Run linters and manually test.

Push to your fork and open a Pull Request.

🧱 Code Standards
🧑‍💻 JavaScript (ES Modules)
Use import/export instead of global scripts.

Prefer modular, reusable, and scoped code.

Avoid polluting the global scope.

Use const and let — never var.

Use arrow functions unless this is needed.

🎯 Naming Conventions
Type	Style	Example
Variables	camelCase	cabLocation, formHandler
Functions	camelCase()	handleBooking(), loadMap()
Constants	UPPER_SNAKE_CASE	MAX_DISTANCE, API_KEY
CSS Classes	BEM	form__input--error
Files	kebab-case	booking-form.js, map.css
Images	kebab-case	cab-icon.png, hero-bg.jpg

🧹 Linting & Formatting
This project uses:

ESLint for JavaScript code quality.

Prettier for consistent code formatting.

✅ Run linters:
bash
Copy
Edit
npx eslint ./js
npx prettier --check .
🛠️ Auto-fix:
bash
Copy
Edit
npx eslint ./js --fix
npx prettier --write .
Make sure your code passes linting and is prettified before opening a PR.

🌐 HTML Guidelines
Use semantic elements (<header>, <main>, <section>, etc.)

Use alt text for all images

Avoid inline styles

Use aria attributes where needed for accessibility

Indentation: 2 spaces

🎨 CSS Guidelines
Follow BEM naming convention

Group CSS by component/module

Use CSS variables if possible (--primary-color)

Keep layout (grid, flexbox) consistent

Avoid overly deep nesting (especially if using SCSS)

🎞️ Animation Guidelines (GSAP)
Group animation logic inside /animations

Use gsap.timeline() for sequencing

Prefer performance-friendly properties: transform, opacity, scale

Use will-change CSS where needed

Avoid animating layout properties like top, left, width dynamically

Keep animations smooth and no longer than necessary

🧠 ES Module Best Practices
Use named exports instead of default if possible

Keep each module focused on one responsibility

Do not use circular imports

Keep pure logic in one place, DOM interaction in another (separation of concerns)

Use tree-shaking-friendly structure:

js
Copy
Edit
// GOOD
export function validateForm() {}
export function clearForm() {}

// BAD
export default {
  validateForm() {},
  clearForm() {}
}
🧪 Testing the Project
🔎 Manual Testing
Since this is a static frontend project:

Open index.html and other pages in browsers:

✅ Chrome

✅ Firefox

✅ Safari

✅ Mobile browser (via DevTools or real device)

Open browser console — make sure there are no errors

Test animations and responsiveness

Test interactive components (form validation, navigation, etc.)

Use W3C Validator for HTML validation

You can optionally use Lighthouse for performance/a11y audits.

🔄 Pull Request Checklist
Before you submit, make sure:

 Code is linted (eslint, prettier)

 Animations are smooth and non-blocking

 HTML is semantic and accessible

 CSS follows BEM and responsive layout tested

 No unused or commented-out code

 No large image or asset bloat

 PR description clearly explains the change

💬 Discuss Before You Code?
Yes — we welcome and encourage opening an issue first for:

Feature ideas

UX or visual redesign suggestions

Major refactors

Adding third-party tools

You don’t need approval for:

Bug fixes

Typo or grammar corrections

Small style fixes

🔐 Security Policy
There is no backend, so data handling is limited, but:

Do not expose any private API keys

Avoid injecting third-party scripts without discussion

Report suspicious behavior or risks via Issues

🔏 Licensing
All contributions will be licensed under the Apache-2.0 License.

By submitting code, you agree to allow the project to use and distribute your contribution under the same license.

🙌 Thank You!
We appreciate your contributions — big or small — and hope you enjoy working on this project. Let’s build a smooth, animated, user-friendly cab booking site together!

Feel free to join the discussions, suggest improvements, or submit pull requests.

Happy coding! 💻🚕
