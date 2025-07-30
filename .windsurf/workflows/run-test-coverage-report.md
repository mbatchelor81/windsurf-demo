---
description: Workflow to remediate failing tests and increase test coverage
---

### Overview: Increase the test coverage by writing new unit tests for low coverage areas 

### 1. Testing & Coverage Workflow
  - Follow these steps to achieve and enforce **≥ 70 % coverage** across the code‑base.
  1. **Run the full suite of jest tests with coverage**
    ```bash
    npm test -- --coverage
    ```
### 2. Fix any failing tests **before** moving on.
  1. **Locate the weakest areas**
    - The coverage summary printed after the first run lists files with the lowest percentages
    - Focus on one file at a time that has the highest 
  2. **Write focused, incremental tests**
    - Target the *lowest‑coverage* files first that have a high impact across the application
    - Analyze the code of the functions, comments and doc strings to reason through the implementation logic
    - Develop a plan to write new unit tests for each of the functions considering edge cases for each function
  3. **Re‑run, refactor, repeat**
    ```bash
    npm test -- --coverage
    ```
### 3. Continue until every file shows **≥ 70 %**.
  1. Continue the workflow until the test coverage has been effectively increased