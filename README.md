# Docs Website

A quick-start template for creating documentation websites using Docsify, with GitHub online editing and automatic deployment.

## Features

- Zero-configuration startup: Begin writing immediately after cloning the repository
- Clean and simple documentation system based on Docsify
- Support for GitHub online editing, facilitating collaboration
- Automatic deployment to GitHub Pages using GitHub Actions
- Pre-set directory structure to help organize your content
- Customizable themes and plugins

## Quick Start Guide

1. Clone your new repository to your local machine.

2. Navigate to the project directory:
```
cd docs-website
```
3. Edit the `docs/home.md` file and other documentation as needed.

4. Commit and push your changes to GitHub:
```
git add .
git commit -m "Update documentation"
git push
```

5. Enable GitHub Pages:
- Go to your repository's Settings
- Navigate to the "Pages" section
- Under "Source", select "GitHub Actions"

## Local Development

To run the website locally:

1. Install docsify-cli globally:
```
npm i docsify-cli -g
```

2. Serve the docs folder:
```
docsify serve docs
```

## Customization
You can customize your documentation website by editing the following files:

- `docs/index.html`: Modify the overall layout and add plugins
- `docs/_sidebar.md`: Edit the sidebar navigation
- `docs/style.css`: Customize the CSS for your website

For more detailed customization options, refer to the [Docsify documentation](https://docsify.js.org/#/).

## GitHub Actions Setup

This template includes a GitHub Action for automatic deployment to GitHub Pages. The action is pre-configured in `.github/workflows/deploy.yml`. You don't need to modify this file unless you want to customize the deployment process.

## How To Set Github Workflow
1. Check repository settings:
Go to your repository settings
Click on "Actions" > "General"
Ensure that the option "Allow GitHub Actions to create and approve pull requests" is checked

2. Check branch protection rules:
In the repository settings, click on "Branches"
If the gh-pages branch has protection rules, make sure the "Allow pushes from GitHub Actions" option is checked

3. Use a Personal Access Token (PAT):
a. Create a new Personal Access Token:
Click on your avatar > Settings > Developer settings > Personal access tokens
Click "Generate new token"
Give the token sufficient permissions (at least repo permission is needed)
Generate and copy this token

b. Add this token as a secret in your repository:
Go to your repository
Click Settings > Secrets > New repository secret
Enter PAT as the name
Enter the token you just generated as the value
Click "Add secret"

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
