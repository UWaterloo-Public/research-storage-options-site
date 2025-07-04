# Research Storage Options Site

A web application for the University of Waterloo that helps researchers find appropriate data storage solutions based on their specific requirements. Built with vanilla JavaScript and designed for easy deployment and maintenance.

-   **Features**: Interactive filtering system, responsive design, CSV data management, real-time search
-   **Limitations**: Static data source (CSV), no user authentication, client-side only
-   **Status**: Active development
-   **Goals**: Provide an accessible tool for UWaterloo researchers to quickly identify appropriate storage solutions based on faculty, data sensitivity, and compliance requirements

## Background

This project was created to address the need for a centralized, user-friendly interface to help University of Waterloo researchers navigate the complex landscape of data storage options. The tool simplifies the decision-making process by allowing users to filter storage solutions based on their specific requirements.

### Environment Requirements

-   Modern web browser with JavaScript enabled
-   Web server (for production deployment) or local file serving capability
-   No backend infrastructure required

### External Dependencies

-   [Papa Parse](https://www.papaparse.com/) - CSV parsing library (included)
-   [Bootstrap](https://getbootstrap.com/) - CSS framework (CDN)

## Development

> This project champions the [UWaterloo software practices](https://uwaterloo-public.github.io/software-development/policies/software-practices.html)

### Setup and Running

1. Clone the repository
2. Open `index.html` in a web browser, or
3. Serve files using a local web server:

    ```bash
    # Using Python
    python -m http.server 8000

    # Using Node.js (if you have http-server installed)
    npx http-server
    ```

4. Navigate to `http://localhost:8000` in your browser

### Testing

-   Manual testing by opening `index.html` and verifying all filtering functionality works
-   Test with different CSV data sets to ensure parsing works correctly
-   Verify responsive design across different screen sizes

## Contributing

We welcome contributions to improve the Research Storage Options Site! Whether you want to:

-   Update storage options data
-   Fix bugs or add new features
-   Improve documentation
-   Enhance the user interface

Please see our [Contributing Guide](CONTRIBUTING.md) for detailed instructions on how to get started, including setup requirements, development workflow, and submission guidelines.

For questions or to report issues, please use [GitHub Issues](../../issues).

## Maintainers

-   campusapps@uwaterloo.ca
-   helpdesk@uwaterloo.ca

## Support

This project uses GitHub issues to track bugs and feature requests. Please search the existing issues before filing new issues to avoid duplicates. For new issues, file your bug or feature request as a new issue.

For help or questions about using this project, please use GitHub issues for general questions and support requests.

**Research Storage Options Site** is under active development and maintained by UWaterloo staff **AND THE COMMUNITY**. We will do our best to respond to support, feature requests, and community questions in a timely manner.
