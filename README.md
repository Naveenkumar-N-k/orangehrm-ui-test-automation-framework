## Project Overview
This project is an UI Test Automation Framework developed to automate the Orange HRM website for UI testing.

The framework follows the **Page Object Model (POM)** design pattern, promoting:
- **Reusability** - Can re-use page object methods across multiple test cases.
- **Scalability** - Easier to extend the framework to accommodate more Page objects & test scenarios.
- **Maintainability** - Keeps the Page objects logic (locators, actions, assertions) separate from test scripts for better organization & easier maintenance.

The framework implements the following test scenario:
- An employee onboarding workflow
  1. Admin login.
  2. Employee registration.
  3. Directory verification.
  4. Login credential validation.

## Playwright Test Report
This is the video recording of the UI automation (showing successful employee onboarding workflow):

https://github.com/user-attachments/assets/f6a50f5a-a2a0-402e-aa17-1bb10b2ea9c9

## Tech Stack
- **Playwright** - Automation framework
- **TypeScript** - Programming language
- **Node.js** - JavaScript runtime environment

## Project Structure
The framework is organized into following components:
- *pages/*: Contains page classes (.ts files) representing different pages in the website. Each class encapsulates it's own locators, actions, assertions, reusable methods (a significant unit of flow is defined in the class methods (composed of actions, locators, assertions)) for interacting with the HTML elements.
- *tests/*: Contains test scripts that utilize the page classes to implement the test cases with the help of re-usable class methods.