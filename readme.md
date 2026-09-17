# 🖥️ QA & Logic: Sort Students - Pure Functions & TypeScript

> ### A strictly typed TypeScript project focusing on immutable data operations, custom sorting algorithms, and pure functions.

This repository demonstrates the ability to write robust, predictable JavaScript/TypeScript logic for data manipulation. 

From a Quality Assurance and Software Engineering perspective, this project showcases how to build pure utility functions that are highly testable, predictable, and safe to use in modern state-management architectures (like Redux or React State), where mutating original data is strictly forbidden.

---

## 🌐 Live Demo & QA Reports

- **[Live Application Demo](#)** *(Replace with your GitHub Pages demo link if applicable)*
- **[Automated Test HTML Report](#)** *(Replace with your test report link)*

---

## 🧪 QA Focus: Design for Testability

Writing testable logic is the foundation of reliable software. This utility was developed with specific constraints to ensure stability in automated Unit Testing environments:

### 1. Immutability & Pure Functions
Flaky tests often occur when functions mutate global state or modify reference parameters. This `sortStudents` function is designed as a **Pure Function**. It uses the spread operator (`[...students]`) to create a shallow copy of the dataset before sorting. 
- **QA Advantage:** Tests can run in any order without "polluting" the original mock data, ensuring 100% predictable test assertions.

### 2. Strict Type Safety (TypeScript)
Dynamic typing in JavaScript can lead to hidden bugs that only appear at runtime. This project implements strict TypeScript structures:
- `Student` interface validates the incoming payload shape.
- `SortType` Enums and `SortOrder` Types strictly define allowed parameters.
- **QA Advantage:** Invalid test data or typo-driven bugs are caught at compile-time by the TS compiler, drastically reducing the required number of defensive runtime unit tests.

### 3. Stable Sorting Algorithm
To prevent test assertions from failing randomly when two students have the exact same sorting value, the algorithm leverages modern JavaScript's **stable sort**. If values are equal, the original array sequence is strictly preserved.

---

## 🎯 Technical Specifications (System Under Test)

The sorting utility handles multiple complex data types and edge cases:

- **String Comparison:** Uses `localeCompare` for names and surnames to ensure accurate, dictionary-order sorting that respects local alphabets and diacritics.
- **Boolean Sorting:** Dynamically casts `boolean` values (`married`) to binary integers (`1` and `0`) to perform mathematical weight comparisons.
- **Derived Data Sorting:** Evaluates the `AverageGrade` on the fly by executing a mathematical reduction (`Array.prototype.reduce`) on a nested array of integers.
- **Dynamic Order Reversal:** Uses a unified ternary logic gate to flip the positive/negative output of the comparison function based on the `asc` or `desc` parameter.

---

## 🧰 Tech Stack

- **Language:** TypeScript / JavaScript (ES6+)
- **Concepts:** Functional Programming (Pure Functions, Immutability), Enums, Interfaces
- **Testing Approach:** Unit Testing compatibility, Edge-case handling

---

## ⚙️ Local Development

1. Clone the repository:
   ```bash
   git clone [https://github.com/webdevnikfull/sort_students.git](https://github.com/webdevnikfull/sort_students.git)
