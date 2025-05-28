## Calculator v2.3 – Test Execution Report

**Tested By**: Mpumelelo Theophilas Nxazonke  
**Date**: 27-05-2025
**Version**: v2.3  
**Priority Issues**: Multiplication (P1), Input Handling (P2)


## Overview

This report summarizes the results of functional and exploratory testing conducted on Calculator v2.3. The key areas of testing included:

## Test Objectives
- Verification of a **known multiplication bug**
- Validation of **addition, division**, and **input error handling**
- Exploratory tests for **edge cases** and **invalid inputs**

Testing was performed manually using the calculator HTML UI and observed outputs.

---

## Conclusion

| **Requirement ID** | **Feature**                | **Test Case**        | **Expected** | **Actual** | **Status**|  
|--------------------|----------------------------|----------------------|--------------|----------- |-----------|
| REQ-44             | UI Version No.             |                      |              |            |           |
| REQ-45             | Addition Accuracy          | 2 + 2                | 4            | 5          |    Fail   |  
| REQ-45             | Addition Accuracy          | 0 + 5                | 5            | 6          |    Fail   |  
| REQ-45             | Addition Accuracy          | 3.1 + 2.2            | 5.3          | 6.3        |    Fail   |  
| REQ-46             | Division Functionality     | 6 / 2                | 3            | 12         |    Fail   |  
| REQ-46             | Division Functionality     | 9 / 3                | 3            | 27         |    Fail   |  
| REQ-46             | Division Functionality     | 5 / 0                | Error        | 0          |    Fail   |  
| REQ-47             | Input Error Handling       | abc + 1              | Error        | blank      |    Fail   |  
| REQ-47             | Input Error Handling       | 5 +                  | Error        | blank      |    Fail   |  
| REQ-47             | Input Error Handling       | 1 ++ 1               | Error        | NaN        |    Fail   |  
| Bug Check          | Multiplication             | 3 * 2                | 6            | 1          |    Fail   |  
| Bug Check          | Multiplication             | 5 * 5                | 25           | 0          |    Fail   |  
| Bug Check          | Multiplication             | -3 * 2               | -6           | -5         |    Fail   |  
| Bug Check          | Multiplication             | 1.2 * 2.5            | 3            | -1.3       |    Fail   |  

All tested areas showed consistent failures due to incorrect handling of mathematical operations and invalid input. The calculator logic incorrectly applies `+1` to addition, treats multiplication as subtraction, and replaces division with multiplication.

---

## Recommendation
- **Correct UI Version No** in the appropriate HTML script
- **Fix core logic bugs** in the `calculate()` function (addition, multiplication, and division).
- Add proper **input validation** for incomplete and malformed expressions.
- Show **user-friendly error messages** for invalid inputs (e.g. “Invalid Expression”).
- Write **unit tests** for calculator logic separately from the UI to isolate bugs.
- Consider implementing **automated test coverage** using Jest or Cypress.

---

## Attachments

### Task 1 Screenshot – Multiplication Bug Confirmation
![Multiplication Bug](./screenshots/task1_multiplication_bug.png)

### Task 2 Screenshot – Division and Input Error Results
![Division & Errors](./screenshots/task2_division_error.png)

### Task 3 Screenshot – Invalid Input Tests
![Invalid Input Tests](./screenshots/task3_invalid_inputs.png)
