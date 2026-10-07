# Maximus - Portfolio

Personal portfolio website for Maximus, a CCT student at Aalborg University.

## Technologies

- HTML
- CSS
- JavaScript
- Git
- GitHub Actions
- Vercel

## Projects

- P1
- P2
- P3
- P4
- P5

## CI/CD Pipeline

This project demonstrates a modern CI/CD workflow.

### Continuous Integration

Every push to `main` and every pull request triggers automated checks.

The deterministic CI checks:

1. Required files exist.
2. The HTML contains the required structure.
3. The portfolio contains the required sections.

### Probabilistic CI

The project can also use an AI-based review step to identify possible issues that deterministic tests may not detect.

AI-based checks are probabilistic because they do not guarantee the same result for every possible change.

### Risk Rule

The pipeline contains a risk rule.

Changes involving:

- GitHub Actions workflows
- Dependencies
- Authentication
- Security

are treated as high-risk changes and require additional review.

### Continuous Deployment

The `main` branch is connected to Vercel.

When an approved change is merged into `main`:

```text
Pull Request
     ↓
Deterministic CI
     ↓
Risk Check
     ↓
Review
     ↓
Merge to main
     ↓
Vercel Deployment
     ↓
Live Portfolio
