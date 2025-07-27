# Ghazal Dib Personal Website

This repository hosts the source code for Ghazal Dib’s personal website, built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/).

## Overview

The site is automatically built and deployed via GitHub Actions workflows whenever changes are pushed or pull requests are opened against the main branch. This ensures fast feedback on build errors and security vulnerabilities before changes are merged.

## Features

- **Automated Build:** The site is built with Jekyll using GitHub Actions on every pull request and push to the main branch.
- **Security Scanning:** Dependency vulnerabilities are detected using `bundler-audit` in a dedicated CI job.
- **Branch Protection:** Merges to the main branch require passing build and security checks to maintain site stability.

## Getting Started

To contribute or customize the website:

1. Fork the repository and create a new branch.
2. Make your changes and test locally with `bundle exec jekyll serve`.
3. Commit and push your changes to your branch.
4. Open a pull request targeting the main branch.
5. Wait for the CI workflows to complete successfully.
6. After approval and passing checks, your changes can be merged.

## Technologies Used

- Ruby 3.2 and Bundler
- Jekyll static site generator
- GitHub Actions for Continuous Integration and Deployment
- Bundler Audit for security scanning

## Workflow Files

- `.github/workflows/jekyll-build.yml` — Builds the site and runs security checks on PRs and pushes.

---

*For any questions or support, please open an issue in this repository.*

