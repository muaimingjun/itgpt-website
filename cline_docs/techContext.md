# Tech Context

## Technologies Used
- **Vue.js:** A progressive JavaScript framework for building user interfaces.
- **Vite:** A modern frontend build tool that provides a faster and leaner development experience.
- **JavaScript (ES6+):** The primary programming language.
- **HTML5 & CSS3:** Standard markup and styling languages for the web.
- **Node.js / npm:** Used for dependency management and running development scripts. The `package.json` file defines project dependencies and scripts.

## Development Environment
- **Local Development Server:** A development server is run using `npm run dev` (a standard Vite command), which provides features like Hot Module Replacement (HMR).
- **Build Process:** The production build is created using `npm run build`, which bundles and optimizes the application for deployment.
- **Code Editor:** The environment suggests the use of VS Code, with visible files and open tabs indicating an active development session.

## Technical Constraints
- **Browser Compatibility:** As a modern web application, it is likely intended for evergreen browsers (latest versions of Chrome, Firefox, Safari, Edge) and may not support older browsers like Internet Explorer.
- **Stateless by Default:** Without a dedicated state management library, complex state sharing between distant components might be challenging.
