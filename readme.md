# 🧪 QA Portfolio: TypeScript Algorithm Validation

> **About this repository:** This project demonstrates White-Box Testing and algorithmic validation using **TypeScript**. It highlights how strong static typing combined with comprehensive unit testing creates bulletproof business logic.

![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Unit Testing](https://img.shields.io/badge/-Unit_Testing-C21325?style=for-the-badge&logo=jest&logoColor=white)
![ESLint](https://img.shields.io/badge/-Static_Analysis-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-CI/CD-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

## 🎯 Project Overview

This repository contains a custom algorithm designed to sort collections of student data (`src/sortStudents.ts`). 

As a **QA Automation Engineer**, my objective in this project is to validate the algorithmic accuracy and handle edge cases at the foundational level of the Testing Pyramid (Unit Tests), leveraging TypeScript's static typing to catch errors at compile-time.

## 🛠️ QA Tech Stack & Tools

* **Core Language:** TypeScript (ES6+)
* **Testing Level:** Unit Testing (White-Box Testing)
* **CI/CD Pipeline:** GitHub Actions (Automated testing on every push/PR)
* **Static Code Analysis (Shift-Left QA):** ESLint tailored for TypeScript

## 📊 Test Strategy & Coverage

The testing strategy isolates the sorting function and validates its behavior against typed data structures:

### 1. Unit Testing (`src/sortStudent.test.ts`)
The automated test suite verifies:
* Correct sorting behavior based on specific student properties (e.g., grades, names, or ID numbers).
* Robust handling of edge cases (e.g., empty arrays, identical values, missing optional properties).
* Adherence to expected data interfaces (ensuring the output strictly matches the defined TypeScript types).

### 2. Static Analysis & Continuous Integration
Integrated with GitHub Actions (`.github/workflows/test.yml`), the CI/CD pipeline enforces a strict quality gate:
* **TypeScript Compilation Check:** Ensures no type errors exist before tests even run.
* **ESLint Verification:** Catches code smells, unused variables, and stylistic issues.
* **Automated Test Execution:** Runs the full unit test suite to prevent regressions.

## 🚀 How to Run the Tests Locally

To evaluate the unit tests and static analysis tools on your local machine, follow these steps:

### 1. Environment Setup
Clone the repository and install the required Node.js dependencies:
```bash
npm install
