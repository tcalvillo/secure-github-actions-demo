
# Secure GitHub Actions CI/CD Demo

## Overview

This project demonstrates the implementation of a secure CI/CD pipeline using GitHub Actions and GitHub Pages while following DevSecOps best practices.

The repository showcases a structured development workflow with separate development, testing, and production branches, automated Continuous Integration (CI), automated deployment (CD), and integrated CodeQL security scanning.

The project serves as both a learning exercise and a portfolio project demonstrating GitHub Actions, workflow security, and modern DevSecOps concepts.

## Features

- Semantic HTML5 website
- Responsive CSS styling
- JavaScript functionality
- Continuous Integration using GitHub Actions
- Automated deployment to GitHub Pages
- Multi-branch promotion strategy
- Pull Request based deployments
- CodeQL security scanning
- Principle of Least Privilege workflow permissions
- GitHub Pages hosting

## Architecture

```text
Developer
     │
     ▼
    dev
     │
 Continuous Integration
     │
     ▼
    test
     │
 Validation
     │
     ▼
    prod
     │
 GitHub Pages Deployment
     │
     ▼
 Live Website
```

## Branching Strategy

| Branch | Purpose |
|---------|---------|
| dev | Active feature development |
| test | Integration testing and validation |
| prod | Production-ready deployment |

## CI/CD Pipeline

### Continuous Integration

The CI workflow performs:

- Repository checkout
- Project structure validation
- HTML/CSS/JavaScript verification

### Continuous Deployment

The deployment workflow:

- Runs only on the `prod` branch
- Publishes the website to GitHub Pages
- Uses secure OIDC authentication

## Security Features

- GitHub CodeQL code scanning
- Least Privilege workflow permissions
- Secure GitHub Pages deployment
- Environment protection
- Pull Request promotion workflow

## Technologies Used

- Git
- GitHub
- GitHub Actions
- GitHub Pages
- HTML5
- CSS3
- JavaScript
- YAML
- CodeQL

## Live Demo

GitHub Pages:

https://tcalvillo.github.io/secure-github-actions-demo/

## Repository Structure

```text
.github/
└── workflows/
    ├── ci.yml
    └── deploy.yml

index.html
style.css
script.js
README.md
LICENSE
```

## Future Improvements

- Add automated unit testing
- Add dependency vulnerability scanning
- Implement Docker-based testing
- Deploy to a cloud platform
- Add Infrastructure as Code (IaC)
- Add release automation

## Lessons Learned

During this project I gained practical experience with:

- Git branching strategies
- Pull Requests and code reviews
- GitHub Actions workflows
- GitHub Pages deployments
- Workflow permissions
- YAML syntax
- Continuous Integration
- Continuous Deployment
- DevSecOps best practices
- Debugging GitHub Actions workflows

## License

This project is licensed under the MIT License.