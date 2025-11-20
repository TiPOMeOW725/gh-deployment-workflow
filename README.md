# GitHub Pages Deployment Workflow

A simple project demonstrating continuous deployment of a static website to GitHub Pages using GitHub Actions.
This project was made as a challenge from roadmap.sh (https://roadmap.sh/projects/github-actions-deployment-workflow).

## Overview

This project automatically deploys changes to `index.html` to GitHub Pages whenever updates are pushed to the `main` branch. It serves as a practical introduction to CI/CD concepts using GitHub Actions.

## Features

- Automated deployment to GitHub Pages
- Triggered on pushes to `main` branch
- Simple static HTML website
- GitHub Actions workflow implementation

## Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/TiPOMeOW725/gh-deployment-workflow
   cd gh-deployment-workflow
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Under "Source", select `gh-pages` branch
   - Click Save

3. **Make changes and push**
   ```bash
   git add .
   git commit -m "Update website"
   git push origin main
   ```

## Project Structure

```
gh-deployment-workflow/
├── .github/
│   └── workflows/
│       └── deploy.yml       # GitHub Actions workflow
├── index.html               # Main HTML file
└── README.md                # Project documentation
```

## How It Works

The GitHub Actions workflow (`.github/workflows/deploy.yml`) automatically:
1. Checks out the repository code
2. Deploys the contents to the `gh-pages` branch
3. GitHub Pages serves the website from the `gh-pages` branch

## Live Demo

Visit the deployed website at: `https://tipomeow725.github.io/gh-deployment-workflow/`

