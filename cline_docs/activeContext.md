# Active Context

## What Is Being Worked On
A comprehensive visual and stylistic overhaul of the "itgpt-website" was undertaken to align its design with the modern, tech-focused aesthetic of `dora.run/ai`.

## Recent Changes
- **Global Styles**: Overhauled `src/assets/base.css` and `src/assets/main.css` to establish a new dark-themed design system with custom fonts (`Inter`, `Sora`), a new color palette, and full-width layout support.
- **Root Component**: Cleaned up `src/App.vue`, removing component-specific styles and logic, and simplifying the template to house the core `Header`, `Hero`, `Features`, and `Footer` components.
- **Header Component**: Rebuilt `src/components/Header.vue` with a "glassmorphism" effect (semi-transparent, blurred background), a new SVG logo, modernized navigation links with hover effects, and a prominent "Get Started" CTA button.
- **Hero Component**: Re-imagined `src/components/Hero.vue` to be a full-viewport, immersive section with a dynamic, animated background, a large, impactful title, and redesigned primary/secondary CTA buttons.
- **Features Component**: Redesigned `src/components/Features.vue` to use a "glassmorphism" card layout with gradient borders and glow effects on hover. Replaced old icons with more modern SVG placeholders.
- **Footer Component**: Re-created `src/components/Footer.vue` with a clean, centered layout, updated links, placeholder social media icons, and a copyright notice.
- **Code Cleanup**: Removed obsolete Vue template files (`HelloWorld.vue`, `TheWelcome.vue`, `WelcomeItem.vue`) and the associated `src/components/icons` directory to keep the project tidy.

## Next Steps
- The visual redesign is complete. The project is now ready for review.
- Awaiting further instructions from the user, which could include populating content, adding more pages/features, or further refining the animations and interactivity.
