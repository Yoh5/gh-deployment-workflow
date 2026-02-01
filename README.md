# gh-deployment-workflow
Roadmap.sh project: Github Actions Deployment Workflow

## Project URL: https://roadmap.sh/projects/github-actions-deployment-workflow

# GitHub Pages Deployment with GitHub Actions

## Project Overview

The goal of this project is to learn and practice the core concepts of **Continuous Integration (CI)** and **Continuous Deployment (CD)** using **GitHub Actions**.

In this project, a simple static website is automatically deployed to **GitHub Pages** whenever changes are made to the `index.html` file on the `main` branch.

This project demonstrates how to:

* Create a GitHub Actions workflow
* Trigger workflows based on file changes
* Deploy a static website automatically
* Use GitHub Pages as a deployment target

---

## Project Requirements

The project fulfills the following requirements:

* A GitHub repository containing:

  * `index.html` (static website)
  * `README.md` (project documentation)
  * `deploy.yml` GitHub Actions workflow
* The workflow runs **only when `index.html` is modified**
* Every valid push to the `main` branch triggers deployment
* The website is accessible via GitHub Pages

Example URL:

```
https://<username>.github.io/gh-deployment-workflow/
```

---

## Project Structure

```text
gh-deployment-workflow/
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml
```

---

## How the CI/CD Pipeline Works

1. A change is pushed to the `main` branch
2. GitHub Actions checks whether `index.html` was modified
3. If yes, the workflow starts
4. The repository is checked out
5. Files are uploaded as an artifact
6. The website is deployed to GitHub Pages automatically

This ensures **continuous deployment** with no manual steps.

---

## GitHub Actions Workflow

The workflow configuration is located at:

```text
.github/workflows/deploy.yml
```

Key features of the workflow:

* Triggered only on `index.html` changes
* Uses official GitHub Pages actions
* Secure permissions setup
* Runs on `ubuntu-latest`

---

## GitHub Pages Setup

To enable GitHub Pages deployment:

1. Go to **Repository Settings**
2. Navigate to **Pages**
3. Under **Source**, select **GitHub Actions**
4. Save the settings

Once enabled, the site will be deployed automatically after each workflow run.

---

## How to Test the Project

1. Clone the repository
2. Modify the content of `index.html`
3. Commit and push the changes to the `main` branch
4. Go to the **Actions** tab and verify the workflow runs successfully
5. Open the GitHub Pages URL to see the updates live

---

## Stretch Goal Ideas

This project can be extended by:

* Using a static site generator (Hugo, Jekyll, Astro)
* Adding a build step before deployment
* Deploying a personal portfolio website
* Adding linting or HTML validation
* Implementing environment-based deployments

---

## Skills Demonstrated

* GitHub Actions
* CI/CD fundamentals
* GitHub Pages deployment
* YAML workflows
* Automation and DevOps basics

---

## Author

Created by **Axel AHo** as a hands-on CI/CD learning project using GitHub Actions.
