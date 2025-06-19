# System Patterns

## How the System Is Built
The system is constructed as a Single-Page Application (SPA) using the Vue.js framework. The project is managed and built using Vite, which provides a fast development server and optimized build process.

## Key Technology Decisions
- **Vue.js:** Chosen as the core front-end framework for its component-based architecture, reactivity, and ease of use.
- **Vite:** Selected as the build tool for its extremely fast Hot Module Replacement (HMR) and efficient production builds.
- **Component-Based Architecture:** The UI is broken down into reusable, self-contained `.vue` components (e.g., `Header.vue`, `Footer.vue`, `Hero.vue`). This promotes modularity and maintainability.
- **Standard Web Technologies:** The project relies on fundamental web technologies: HTML, CSS, and JavaScript (ES6+).

## Architectural Patterns
The primary architectural pattern is **Component-Based Architecture**. The application's UI is composed of a tree of nested components, with `App.vue` serving as the root component. State management appears to be handled locally within components, as there is no evidence of a global state management library like Vuex or Pinia in the file structure.
