---
description: Run and validate test success and repo coverage
---

## Follow the steps below to run tests and go through necessary steps to remediate.

1. Run the tests in this repository and fix any failing tests.
```bash
npm run test:coverage
```

2. Write new test cases to increase the test coverage starting with files that have lowest coverage.

3. Remediate the new test cases, and repeat these steps until the test coverage for all files is greater than 70 percent.