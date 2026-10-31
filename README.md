# HMCTS Caseworker Task Management System – Frontend

## Project Overview

This project provides the frontend for the HMCTS Caseworker Task Management System. It enables caseworkers to create, view and manage tasks through a web-based interface.

The frontend communicates with the backend REST API to retrieve and manage task information.

## Technology Stack

- Node.js
- TypeScript
- Express.js
- Nunjucks
- GOV.UK Design System / GOV.UK Frontend
- SCSS
- Webpack
- Jest

## Prerequisites

The following environment was used to build and test the frontend successfully:

- Node.js: `24.22.2`
- Yarn: `4.16.0`

### Node.js setup

Install and activate the tested Node.js version using NVM:

```bash
nvm install 24.22.2
nvm use 24.22.2
```

Verify the installed versions:

```bash
node --version
yarn --version
```

## Getting Started

### 1. Clone the repository

```bash
git clone <repository-url>
cd hmcts-dev-test-frontend
```

### 2. Install dependencies

```bash
yarn install
```

### 3. Build the frontend

```bash
yarn webpack
```

### 4. Run build and quality checks

```bash
yarn cichecks
```

This runs dependency installation, the Webpack build, Puppeteer rebuild, linting, formatting checks, unit tests and route tests.

### 5. Start the development server

```bash
yarn start:dev
```

Open the local URL displayed in the terminal to access the application.

## Available Commands for reference

| Purpose | Command |
|---|---|
| Build frontend | `yarn webpack` |
| Start development server | `yarn start:dev` |
| Run all CI checks | `yarn cichecks` |
| Run linting and formatting | `yarn lint` |
| Run unit tests | `yarn test:unit` |
| Run route tests | `yarn test:routes` |
| Run functional tests | `yarn test:functional` |
| Generate test coverage | `yarn test:coverage` |

## Backend Integration

The frontend communicates with the backend REST API to retrieve and manage task information.

Ensure the backend service is running and correctly configured when testing functionality that requires API access.