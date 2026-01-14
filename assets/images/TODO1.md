# TODO: Enhance Portfolio with Projects Visualizations and Certifications Carousel

## Overview
This TODO outlines the steps to implement suggestions for adding multiple projects with visualizations (pictures and brief explanations) and certifications in a carousel form with verification marks and logos. The goal is to enhance UX while maintaining consistency with the existing codebase.

1. Enhance Portfolio Section for Multiple Projects with Visualizations
   - **1.1 Update HTML Structure**
     - Modify each `.project-item > a` in the portfolio section to include data attributes for modal triggering (e.g., `data-project-modal`).
     - Add a new modal container for projects (reuse and adapt the testimonials modal structure) with placeholders for larger images, descriptions, tech stacks, and links.
   - **1.2 Update CSS Styles**
     - Extend `.testimonials-modal` styles for project modals to ensure responsiveness and overlay behavior.
     - Add hover effects for project items (e.g., scale image, reveal icon).
     - Ensure modal content (images, text) is styled consistently with existing cards.
   - **1.3 Update JavaScript Functionality**
     - Add event listeners to project items to populate and show the modal (extend `testimonialsModalFunc`).
     - Populate modal with dynamic content: larger image, brief description (2-3 sentences), optional tech stack icons, demo/repo links.
     - Test modal open/close and overlay interactions.
   - **1.4 Add Project Content**
     - Populate project items with actual data: images, titles, categories, and modal details.
     - Add new filter categories if needed (e.g., "Data Science", "AI/ML") based on skills section.

## 2. Add Certifications Section in Carousel Form
   - **2.1 Update HTML Structure**
     - Add a new `<article class="certifications" data-page="certifications">` after the portfolio article.
     - Include a header with title (e.g., "Certifications").
     - Create a horizontal scrollable list (`.certifications-list`) with cards for each certification: thumbnail image, title, issuer, date.
     - Add verification marks (e.g., blue/gold icons) and issuer logos overlaid on images.
   - **2.2 Update CSS Styles**
     - Style certification cards using `.content-card` for consistency.
     - Implement carousel scrolling with `.has-scrollbar` and add smooth transitions.
     - Position verification marks (e.g., using pseudo-elements or icons) and logos (e.g., bottom-right overlay).
     - Ensure mobile responsiveness with existing media queries.
   - **2.3 Update JavaScript Functionality**
     - Add "Certifications" to navbar links and pages array for navigation.
     - Implement carousel auto-scroll or button controls if desired (extend filter/select logic).
     - Add click handlers for certification items (e.g., enlarge image in modal).
   - **2.4 Add Certification Content**
     - Populate with actual certifications: images, titles, issuers, dates.
     - Select and apply verification mark styles (blue for standard, gold for premium).

## 3. General Enhancements and Testing
   - **3.1 Accessibility and Performance**
     - Add alt text to all new images and ARIA labels for modals/carousels.
     - Optimize images (e.g., WebP format, lazy loading).
   - **3.2 Testing**
     - Test navigation between sections (About, Portfolio, Certifications, Contact).
     - Verify modal interactions, carousel scrolling, and filter functionality on desktop and mobile.
     - Check for layout breaks and ensure dark theme consistency.
     - Perform thorough testing: Navigate all pages, interact with all elements, test edge cases (e.g., empty modals).
   - **3.3 Final Review**
     - Review overall UX: Ensure explanations are brief, visualizations are engaging, and verification marks/logos enhance credibility.
     - Update any documentation or comments in code.

## Dependencies
- Reuse existing classes: `.content-card`, `.has-scrollbar`, `.modal-container`.
- Ensure compatibility with current JS navigation and modal systems.
- No new libraries needed; leverage IonIcons for marks/logos.

## Next Steps
- Prioritize based on user feedback (e.g., start with portfolio enhancements).
- After each major step, test incrementally to avoid issues.
- If content (images, descriptions) is not ready, placeholders can be used initially.

- publish soon
