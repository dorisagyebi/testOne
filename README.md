# Playwright TodoMVC Test Suite

## Overview
This project contains a test suite written in Playwright to validate the functionality of the TodoMVC application.
The tests cover various scenarios, including adding, editing, completing, and deleting todo items, ensuring the application's reliability.

## Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (LTS recommended)
- [Playwright](https://playwright.dev/)

## Installation
1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd <project-directory>
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Install Playwright browsers:
   ```sh
   npx playwright install
   ```

## Running Tests
Execute the test suite using:
```sh
npx playwright test
```
To run a specific test file:
```sh
npx playwright test tests/todo.test.js
```

## Test Scenarios Covered
- Adding new todo items
- Clearing input after adding a task
- Marking tasks as complete/incomplete
- Editing and deleting tasks
- Ensuring correct UI updates
- Persisting data in local storage

## Folder Structure
- `tests/` - Contains all Playwright test cases
- `package.json` - Project dependencies and scripts
- `playwright.config.ts` - Playwright configuration file

## Debugging Tests
To run tests in headed mode for debugging:
```sh
npx playwright test --headed
```
To trace test execution:
```sh
npx playwright test --trace on
```

## Reporting
Generate an HTML report after test execution:
```sh
npx playwright test --reporter=html
```
Open the report:
```sh
npx playwright show-report
```



