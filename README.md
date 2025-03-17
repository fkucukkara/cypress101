# Cypress 101

Welcome to Cypress 101! This project is a boilerplate setup for end-to-end testing using Cypress.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Writing Tests](#writing-tests)
- [Running Tests](#running-tests)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Cypress 101 is a starter project to help you get up and running with Cypress for end-to-end testing. It includes basic configurations and examples to demonstrate how to write and run tests using Cypress.

## Installation

To get started, clone the repository and install the dependencies:

```bash
git clone https://github.com/fkucukkara/cypress101.git
cd cypress101
npm install
```

## Usage

After installing the dependencies, you can open Cypress and start writing your tests.

```bash
npx cypress open
```

This will open the Cypress Test Runner, where you can see and run your tests.

## Project Structure

Here is an overview of the project structure:

```
cypress101/
├── cypress/
│   ├── e2e/
│   │   └── spec.cy.js
│   ├── fixtures/
│   │   └── example.json
│   ├── support/
│   │   ├── commands.js
│   │   └── e2e.js
├── node_modules/
├── .gitignore
├── cypress.config.js
├── package.json
└── README.md
```

- `cypress/e2e/`: Contains the test specifications.
- `cypress/fixtures/`: Contains test data files.
- `cypress/support/`: Contains support files for custom commands and global configurations.
- `cypress.config.js`: Cypress configuration file.
- `package.json`: Project dependencies and scripts.

## Writing Tests

Tests are written in JavaScript and are located in the `cypress/e2e/` directory. Here is an example test:

```javascript
describe('template spec', () => {
  it('passes', () => {
    cy.visit('https://example.cypress.io')
  })
})
```

## Running Tests

You can run tests in headless mode using the following command:

```bash
npx cypress run
```

This will run all the tests and output the results in the terminal.
