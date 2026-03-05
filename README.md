# Opnigma Website Prototype

This folder contains the complete design system and static HTML/CSS/JS implementation for the Opnigma website, built strictly according to your guidelines. It is designed specifically to be easily ported into **Elementor Pro** in WordPress while ensuring a highly premium, modern look that matches NorthStar’s supply chain tech positioning.

## Folders & Files
- `/assets/css/style.css`: All the core styles, including Elementor-ready CSS variables for global colors, typography, and spacing.
- `/assets/js/main.js`: Smooth scrolling, sticky header toggles, and mobile menu logic.
- `index.html`: The main single-page layout containing Hero, Services, ROI, Approach, and Contact sections mapped to anchors.
- `about.html`: Our Story and Values.
- `use-cases.html`: The Use Cases layout featuring PDF downloads and detailed ROI metrics.

## Elementor Pro Translation Guide

When you import this design into WordPress + Elementor Pro, here is the suggested workflow:

1. **Global Site Settings**:
   - Navigate to Elementor > Site Settings.
   - Set the **Global Colors**:
     - `Primary`: `#0b2447` (Dark Blue)
     - `Secondary`: `#e63946` (Accent Red)
     - `Text`: `#1e293b`
     - `Accent`: `#457b9d`
   - Set the **Global Fonts**:
     - Primary Heading / Secondary Heading: `Outfit` (700, 800 weight)
     - Body Text: `Inter` (400, 500 weight)

2. **Template Builder**:
   - Use **Elementor Theme Builder** to create the Header and Footer templates so they inherit on all pages (`index.html`, `about.html`, `use-cases.html`).
   - The header should have a Sticky motion effect enabled (`Motion Effects > Sticky: Top`).

3. **Homepage Layout (`index.html`)**:
   - The sections in `index.html` translate 1:1 to **Elementor Sections/Containers**.
   - Assign `CSS ID` to each main container (e.g. `services`, `use-cases`, `approach`, `platform`, `contact`) so the header navigation works as anchor links.

4. **Dynamic Data & CMS (Custom Post Types)**:
   - For **Use Cases**, create a Custom Post Type using ACF/CPT UI and create an Elementor Loop Grid / Custom Skin to handle the cards dynamically as built in `use-cases.html`. The FR8Focus PDF can be an ACF File field.
   - For **Services**, these can be built as icon boxes or image boxes in a CSS Grid (Elementor Grid Container) or an individual CPT if they will expand.

5. **Contact Form**:
   - Use the native Elementor Form widget. The layout provided in `index.html` maps to a standard Elementor Form with Name, Company, Email, Select dropdown, Textarea, and Checkbox.
   - Connect the Form Actions to native email notifications or a CRM like HubSpot via the integrations tab.

## Design Highlights
- **Typography and Aesthetics**: Deep tech blues with striking red accents, paired with high-tech warehouse imagery, delivering an authoritative and futuristic supply chain vibe.
- **Glassmorphism & Gradients**: Subtle backdrops and gradients are used behind forms and stats to elevate perceived value.
- **Micro-interactions**: Hover effects on cards, navigation, and buttons ensure the site feels deeply interactive.

*Built based on the provided NorthStar inspiration, Opnigma front page ideas, and the Review documentation.*
