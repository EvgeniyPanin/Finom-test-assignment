# Finom Test Assignment

This project is a test task for the **Finom** company. It demonstrates a simple, responsive banner component for business funding, built with semantic HTML and modular CSS.

## Project Structure

- **index.html**: Main HTML file containing the banner markup and minimal JavaScript for banner dismissal.
- **main.css**: Contains all styles, structured for scalability and maintainability.
- **normalize.css**: CSS reset for cross-browser consistency.
- **public/**: Folder for static assets (SVGs, images).

## CSS Structure

The CSS is organized using the [BEM (Block Element Modifier)](http://getbem.com/) methodology, which helps keep styles modular and readable.  
For example:  
- `.banner`, `.banner__title`, `.banner__actions`, `.list__item`, etc.

### Helper Classes

To avoid repetition and keep the CSS bundle size small (especially important for SSR projects), several helper classes are included:
- `.f-w-500`, `.f-w-600`: Font weight utilities.
- `.t-a-center`: Text alignment.
- `.uppercase`: Text transformation.

These can be reused across components and pages, making the codebase more maintainable.

### Reusable Components

The following reusable components are implemented:
- **Paper**: `.paper` — Card-like container with padding and rounded corners.
- **Button**: `.button` — Styled action button.
- **Close Button**: `.close-button` — Icon-only button for dismissing the banner, with an accessible `aria-label`.
- **List**: `.list`, `.list__item` — Custom-styled list with icons.

## Accessibility

The close button uses an `aria-label` attribute to ensure it is accessible to screen readers, since it does not contain visible text.