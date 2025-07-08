# AGENTS.md

This file provides AI coding agents with structured information about the Research Storage Options Site project to ensure consistent, high-quality code generation and task execution.

## Project Overview

**Project Name**: Research Storage Options Site  
**Type**: Static Web Application  
**Primary Language**: JavaScript (ES6+)  
**Framework**: Vanilla JavaScript with Bootstrap CSS  
**Target Audience**: University of Waterloo researchers  
**Purpose**: Interactive tool to help researchers find appropriate data storage solutions based on their requirements

## Architecture & Technology Stack

### Core Technologies

-   **Frontend**: Vanilla JavaScript (ES6+), HTML5, CSS3
-   **CSS Framework**: Bootstrap 5.3.2 (CDN)
-   **Data Processing**: Papa Parse library for CSV parsing
-   **Data Source**: CSV file (`storage2.csv`)
-   **Deployment**: Static hosting (no backend required)

### File Structure

```
/
├── index.html              # Main application file (HTML + CSS + JS)
├── storage2.csv           # Data source for storage options
├── papaparse.min.js       # CSV parsing library
├── favicon.ico            # Site favicon
├── logo.png               # UWaterloo logo
├── uwaterloo-logo.svg     # UWaterloo SVG logo
├── README.md              # Project documentation
├── LICENSE                # Project license
├── CODE_OF_CONDUCT.md     # Community guidelines
├── CONTRIBUTING.md        # Contribution guidelines
└── SECURITY.md            # Security policies
```

## Coding Standards & Conventions

### JavaScript Style

-   Use ES6+ features (const/let, arrow functions, template literals)
-   Function names should be descriptive and use camelCase
-   Use vanilla JavaScript - avoid jQuery or other heavy frameworks
-   All code should be contained within `index.html` for simplicity
-   Comment complex logic clearly

### CSS Standards

-   Use CSS custom properties (variables) for theming
-   Follow University of Waterloo brand colors:
    -   `--waterloo-gold: #fed34c`
    -   `--waterloo-black: #000000`
    -   `--waterloo-dark-gray: #333333`
    -   `--waterloo-light-gray: #f8f9fa`
-   Use Bootstrap classes where possible, custom CSS for specific needs
-   Responsive design is mandatory (mobile-first approach)

### HTML Standards

-   Semantic HTML5 elements
-   Accessibility attributes (aria-labels, roles)
-   Proper form structure with labels
-   University of Waterloo branding elements

## Data Management

### CSV Data Structure

The `storage2.csv` file contains:

-   **Column 1**: Question categories
-   **Column 2**: Option values
-   **Column 3**: Hover-over notes
-   **Column 4**: Reference links
-   **Columns 5+**: Storage solution compatibility (1=compatible, 0=not compatible)

### Data Processing Rules

-   Use Papa Parse library for CSV parsing
-   First row contains headers/storage solution names
-   Process boolean values (1/0) for filtering logic
-   Handle special cases like "Contact Information Security Services" text
-   Maintain data integrity during filtering operations

## Core Functionality

### Main Features

1. **Multi-criteria Filtering**: Users can filter by faculty, data classification, storage needs, etc.
2. **Real-time Results**: Dynamic updating of compatible storage options
3. **Responsive Design**: Works on desktop and mobile devices
4. **University Branding**: Consistent UWaterloo visual identity

### Key Functions

-   `processCSV(data)`: Parses CSV and builds filter options
-   `updateResults()`: Applies filters and displays compatible storage solutions
-   `resetForm()`: Clears all filters and resets the interface

## Development Guidelines

### When Adding Features

1. Maintain the single-file architecture (`index.html`)
2. Follow University of Waterloo design patterns
3. Ensure accessibility compliance
4. Test across different browsers and devices
5. Validate with sample CSV data

### When Modifying Data Structure

1. Update CSV parsing logic in `processCSV()` function
2. Ensure column mapping remains consistent
3. Test filtering logic with new data fields
4. Update documentation if schema changes

### When Styling

1. Use existing CSS custom properties
2. Maintain Bootstrap responsive grid system
3. Follow University of Waterloo brand guidelines
4. Ensure contrast ratios meet accessibility standards

## Dependencies & External Resources

### CDN Dependencies

-   Bootstrap 5.3.2 CSS: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css`
-   Bootstrap 5.3.2 JS: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js`

### Local Dependencies

-   Papa Parse library (`papaparse.min.js`) - Must remain local for offline functionality

### University Resources

-   Official UWaterloo logos and branding elements
-   Links to university storage service documentation
-   Compliance with university web policies

## Testing & Quality Assurance

### Manual Testing Checklist

-   [ ] All filters work independently and in combination
-   [ ] Results update correctly when filters change
-   [ ] Reset functionality clears all selections
-   [ ] Responsive design works on mobile devices
-   [ ] All external links are functional
-   [ ] CSV data loads and parses correctly

### Browser Compatibility

-   Target: Modern browsers (Chrome, Firefox, Safari, Edge)
-   Minimum: ES6 support required
-   Mobile: iOS Safari, Android Chrome

## Deployment

### Local Development

```bash
# Serve locally using Python
python -m http.server 8000

# Or using Node.js
npx http-server
```

### Production Deployment

-   Static hosting compatible (GitHub Pages, Netlify, etc.)
-   No build process required
-   Ensure all assets are properly linked with relative paths
-   Test CSV loading in production environment

## Security Considerations

### Data Handling

-   All processing happens client-side
-   No user data is stored or transmitted
-   CSV data should be validated before deployment
-   Follow university data governance policies

### Content Security

-   Use HTTPS in production
-   Validate all external links regularly
-   Follow university security guidelines for web applications

## Common Tasks for AI Agents

### Adding New Storage Options

1. Update `storage2.csv` with new column for the storage solution
2. Add compatibility ratings (1/0) for each filter criteria
3. Include proper documentation links
4. Test filtering logic with new option

### Modifying Filter Categories

1. Update CSV structure if needed
2. Modify `processCSV()` function to handle new categories
3. Update HTML form elements
4. Adjust filtering logic in `updateResults()`

### UI/UX Improvements

1. Maintain University of Waterloo branding
2. Use Bootstrap components for consistency
3. Ensure accessibility compliance
4. Test responsive behavior

### Performance Optimization

1. Keep JavaScript vanilla for minimal overhead
2. Optimize CSV parsing for larger datasets
3. Use efficient DOM manipulation techniques
4. Monitor load times and optimize as needed

## Contact & Support

For questions about University of Waterloo requirements, branding, or data governance, refer to:

-   University web policies and guidelines
-   IST service documentation
-   Faculty-specific IT support contacts as listed in the CSV data

---

_This AGENTS.md file should be updated whenever significant architectural changes are made to ensure AI agents have current information about the project._
