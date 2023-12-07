![NestJS Logo](https://nestjs.com/img/logo_text.svg)

# @iamtalwinder/nestjs-package-starter

🚀 **NestJS Package Starter**: A streamlined, ready-to-use template for building robust, scalable NestJS packages.

## Description

This package provides a well-structured template that’s ideal for kickstarting the development of NestJS modules. It’s equipped with essential configurations and a flexible structure to elevate your NestJS ecosystem.

## Features

- Ready-to-use structure for NestJS modules.
- Essential configurations for TypeScript, Jest, ESLint, and Prettier.
- Integrated testing setup with Jest.
- Continuous Integration and Release Management with `release-it`.

Certainly! Below is the continuation of your `README.md` with instructions on how to create a new package by cloning your starter template, modifying the code, and preparing it for release:

---

## Getting Started with Your Own Package

Follow these steps to use this starter template to create your own NestJS package:

### Step 1: Clone the Repository

First, clone the `nestjs-package-starter` repository:

```bash
git clone https://github.com/iamtalwinder/nestjs-package-starter.git your-package-name
cd your-package-name
```

Replace `your-package-name` with the name of your new package.

### Step 2: Install Dependencies

Install the necessary dependencies:

```bash
npm install
```

### Step 3: Modify the Package

- **Update Package Details**: Edit the `package.json` file to reflect your package's name, description, repository, etc.
- **Develop Your Module**: Add or modify the NestJS modules, services, etc., inside the `lib` directory.
- **Write Tests**: Write unit and end-to-end tests for your modules inside the `test` directory. Place unit tests in `test/unit` and end-to-end tests in `test/e2e`.

### Step 4: Run and Test Locally

Before publishing, you can build and test your package locally:

- **Build Your Package**: Run `npm run build` to compile your TypeScript code.
- **Run Unit Tests**: Execute `npm run test:unit` to run unit tests.
- **Run E2E Tests**: Execute `npm run test:e2e` to run end-to-end tests.

### Step 5: Prepare for Release

To prepare your package for release, follow these steps:

1. **Set Up Git Repository**: Initialize a new Git repository if you haven't already:

    ```bash
    git init
    git add .
    git commit -m "Initial commit"
    ```

2. **Configure `release-it`**: If not already configured, set up `release-it` in your project. You might want to modify `.release-it.json` to suit your release workflow.

Absolutely, setting up the remote repository correctly is an important step in managing your package's source code and preparing for publication. Here are the steps including the ones you mentioned, to be added in your `README.md`:

### Step 6: Set Up Remote Repository

Before you release and publish your package, make sure your local repository is properly linked to a remote repository on GitHub (or another version control service). This step is crucial for version control and collaboration.

1. **Create a Remote Repository**: If you haven't already, create a new repository on GitHub (or your preferred service). Do not initialize it with a README, license, or .gitignore files — your local repository will already have these.

2. **Add Remote Repository**: Link your local repository to the remote repository. Replace `<github_url>` with the URL of your new GitHub repository.

    ```bash
    git remote add upstream <github_url>
    ```

3. **Push to Remote Repository**: Push your code to the main branch of the remote repository. This step uploads your local repository content to GitHub.

    ```bash
    git push --set-upstream origin main
    ```

Remember to replace `<github_url>` with the actual URL of your GitHub repository. These instructions will guide users through setting up their own package, pushing it to a remote repository, and publishing it to npm.

### Step 7: Publish Your Package

**Create a Release**: When you're ready to publish your package, you can use `release-it` to automate the versioning and publishing process:

    ```bash
    npm run release
    ```

 This command will handle version bumping, tagging, and publishing your package to npm. Ensure you have the correct access rights on npm and your Git remote is set up correctly.
