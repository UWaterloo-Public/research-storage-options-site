## GRANT OF LICENSE - PLEASE READ!

By contributing to this repository, you agree to grant a non-exclusive,
royalty-free, and irrevocable license to the University of Waterloo
for your contributions.

You also agree to irrevocably waive any other rights related to your
contributions, such as moral rights, which could restrict the University's
subsequent use and distribution of software which contains your contributions.

This means that the University can use and modify your contributions
without restriction, and further distribute any software that contains
your contributions without seeking additional permission from you.

Should you have any concerns with the terms of this grant of license,
please do not proceed with any changes.

The current terms of license applicable to this project are contained
in the LICENSE file included in the Repository. Please note that the
University may change the licensing terms applicable to the software
without further notice, for instance, from closed source to open source
(and vice versa).

## Contributing guide

Hi there! We're thrilled that you'd like to contribute to this project. Your help is essential for keeping it great.

Contributions to this project are released to the public under this [project's license](LICENSE).

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## Prerequisites for running and testing code

These are one time installations required to be able to test your changes locally as part of the pull request (PR) submission process.

1. **Modern web browser** - Chrome, Firefox, Safari, or Edge (latest versions recommended)
2. **Text editor** - Any code editor (VS Code, Sublime Text, etc.) for making changes
3. **Basic understanding of HTML, CSS, and JavaScript** - For code contributions
4. **CSV editing knowledge** - For data updates (Excel, Google Sheets, or text editor)

## Submitting a pull request

### Standard workflow

1. **Fork the Repository**

    - Navigate to the GitHub repository
    - Click the "Fork" button in the top-right corner to create your own copy

2. **Clone Your Fork**

    ```bash
    git clone https://github.com/YOUR-USERNAME/research-storage-options-site.git
    cd research-storage-options-site
    ```

3. **Test your setup**: Open `index.html` in your web browser to ensure the application loads and functions correctly

4. **Create a New Branch**

    ```bash
    git checkout -b feature/your-feature-name
    # or
    git checkout -b fix/your-bug-fix
    ```

5. **Make Your Changes**

    - Edit files directly in your code editor
    - Test your changes by refreshing `index.html` in your browser
    - Ensure all functionality works as expected

6. **Commit Your Changes**

    ```bash
    git add .
    git commit -m "Descriptive commit message about your changes"
    ```

7. **Push to Your Fork**

    ```bash
    git push origin feature/your-feature-name
    ```

8. **Create a Pull Request**
    - Go to your fork on GitHub
    - Click "New Pull Request"
    - Provide a clear description of your changes
    - Submit the pull request for review

### Making Quick Edits on GitHub

For small changes like updating documentation or fixing typos:

1. **Navigate to the file** you want to edit on GitHub
2. **Click the pencil icon** (✏️) in the top-right corner of the file view
3. **Make your changes** in the web editor
4. **Add a commit message** describing your changes
5. **Choose "Create a new branch"** and start a pull request
6. **Submit the pull request** for review

## Types of Contributions

-   **Data Updates**: Add new storage options or update existing ones in `storage2.csv`
-   **Bug Fixes**: Fix issues with filtering, display, or functionality
-   **Feature Enhancements**: Add new filtering options, improve UI/UX
-   **Documentation**: Improve README, add code comments, or create user guides
-   **Performance**: Optimize loading times or improve responsiveness

## Guidelines

## Guidelines

-   **Follow consistent formatting** - Use proper indentation, maintain existing code style
-   **Test thoroughly** - Verify all functionality works after your changes
-   **Keep CSV data clean** - Ensure proper formatting and no missing required fields
-   Keep your change as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
-   Update documentation if you're adding new features
-   Be respectful and constructive in pull request discussions
-   Write a [good commit message](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

## Questions or Issues?

-   **Report bugs** by opening an issue on GitHub
-   **Suggest features** through GitHub issues
-   **Ask questions** in issue discussions or pull request comments
