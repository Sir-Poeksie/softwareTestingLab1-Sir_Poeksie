# 🐞 Test Summary Report TEMPLATE
**Copy-paste this when creating new [issues](https://github.com/PLP-Database-DEPT/swt-01/issues)**:

```markdown

## Test Coverage Report  

| Requirement | Test Cases       | Pass/Fail | Notes               |  
|-------------|------------------|-----------|---------------------|  
| REQ-45      | `x + y`, `r + h` | 1/2 Pass  | Addition bug found  |  
| REQ-46      |                  |           |                     |  
| REQ-47      |                  |           |                     |  
# 📊 Test Summary Table

| Test Case      | Requirement | Expected | Actual | Status | Notes                           |
|----------------|-------------|----------|--------|--------|---------------------------------|
| 2 + 2          | REQ-45      | 4        | 5      |  Fail  | Off-by-one addition bug         |
| 0 + 5          | REQ-45      | 5        | 6      |  Fail  | Same addition bug               |
| 3 * 2          | REQ-XX      | 6        | 1      |  Fail  | Multiplication = Subtraction    |
| 5 * 0          | REQ-XX      | 0        | 5      |  Fail  | Logic error                     |
| -3 * 2         | REQ-XX      | -6       | -5     |  Fail  | Logic error                     |
| 1.2 * 2.5      | REQ-XX      | 3        | -1.3   |  Fail  | Floating point bug              |
| 6 / 2          | REQ-46      | 3        | 3      |  Pass  |                                 |
| 7 / 2          | REQ-46      | 3.5      | 3.5    |  Pass  |                                 |
| 5 / 0          | REQ-46      | Error    | 0      |  Fail  | Should handle divide-by-zero    |
| abc + 1        | REQ-47      | Error    | 1      |  Fail  | No input validation             |
| 5 +            | REQ-47      | Error    | 5      |  Fail  | No error on incomplete input    |
| 1 ++ 1         | REQ-47      | Error    | 3      |  Fail  | Invalid syntax misparsed        |
