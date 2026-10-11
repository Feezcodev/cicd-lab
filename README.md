
# CI/CD Lab — Automated Testing & Deployment

A hands-on DevOps project focused on building a reliable CI/CD pipeline for a Node.js and TypeScript application using automated testing, GitHub Actions, and cloud deployment.

This project demonstrates my practical learning journey in **Continuous Integration, Continuous Delivery, automation, application testing, and deployment workflows**.

The goal is to build a repeatable pipeline that validates application changes before they are deployed, helping improve software quality and release reliability.

## Project Overview

The CI/CD Lab is an Express.js and TypeScript application that serves as the foundation for implementing an automated software delivery pipeline.

I am extending this project step by step to practise real-world DevOps workflows, from local development and automated testing to continuous integration and cloud deployment.

## Tech Stack

- **Application:** Node.js 24, Express.js, TypeScript
- **Package Management:** npm
- **Version Control:** Git and GitHub
- **Testing:** Automated health endpoint tests
- **CI/CD:** GitHub Actions (implementation in progress)
- **Deployment:** Render (planned as part of the lab)
- **Build & Validation:** TypeScript type checking and compilation

## Current Features

- Express.js application with a home page.
- Health check endpoint for basic application health verification.
- Automated test for the health endpoint.
- TypeScript type checking without generating build output.
- Production build process that compiles the application into `dist`.
- Separate development and production start commands.

## Getting Started

### Prerequisites

Install the following tools before running the project:

- Node.js 24 and npm
- Git
- A GitHub account

A Render account will be needed for the deployment stage.

### 1. Clone the Repository

```bash
git clone https://github.com/Feezcodev/cicd-lab.git
cd cicd-lab
```

### 2. Install Dependencies

```bash
npm ci
```

### 3. Start the Development Server

```bash
npm run dev
```

The application runs locally on port `3000` by default.

Open the following endpoints in your browser:

- Home page: http://localhost:3000
- Health check: http://localhost:3000/api/health

Expected health check response:

```json
{
  "status": "ok"
}
```

Stop the development server with `Ctrl + C`.

## Available Commands

| Command | Purpose |
|---|---|
| `npm run dev` | Start the development server |
| `npm run typecheck` | Check TypeScript types |
| `npm test` | Run automated tests |
| `npm run build` | Compile the application |
| `npm start` | Start the compiled application |

## DevOps Implementation Roadmap

I am using this project to build and demonstrate practical experience with the following workflows.

### Phase 1 — Application Validation

- Run TypeScript type checking.
- Execute automated tests.
- Build the application for production.
- Identify failures before deployment.

### Phase 2 — CI/CD with GitHub Actions

- Create a GitHub Actions workflow.
- Trigger pipeline execution on code pushes and pull requests.
- Install dependencies using the committed lockfile.
- Run verification checks and automated tests.
- Build the application and fail the workflow when required checks fail.

### Phase 3 — Application Versioning

- Implement a version endpoint.
- Expose application version information for verification.
- Validate the running application after deployment.

### Phase 4 — Cloud Deployment

- Configure the application for deployment on Render.
- Deploy the application from the GitHub repository.
- Configure required environment variables.
- Verify the deployed application using its health endpoint.
- Practise troubleshooting failed builds and deployment issues.

*Implementation status: This roadmap describes the planned learning objectives. Individual phases will be marked complete as they are implemented and tested.*

## What I'm Learning

Through this project, I am developing practical skills in:

- CI/CD pipeline design and implementation.
- Automated testing and build validation.
- Git-based version control workflows.
- TypeScript application build processes.
- Environment variable configuration.
- Cloud application deployment and health verification.
- Troubleshooting failures across the software delivery lifecycle.

## Future Improvements

As the project evolves, I plan to explore:

- Pull request quality gates.
- Build artifact management.
- Deployment verification and rollback strategies.
- Containerization with Docker.
- Infrastructure automation with Terraform.
- Security scanning within CI/CD pipelines.

## Repository

**GitHub:** https://github.com/Feezcodev/cicd-lab

## About Me

I am building my career in DevOps, Cloud Engineering, and Platform Engineering through hands-on projects focused on automation, infrastructure, CI/CD, and reliable application delivery.

I believe in learning by building, documenting what I implement, and continuously improving my engineering skills.

**One project. One skill. One opportunity at a time.**

Connect with me on GitHub: https://github.com/Feezcodev
