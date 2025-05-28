# 🐞 New Discovery Report TEMPLATE
**Copy-paste this when creating new [issues](https://github.com/PLP-Database-DEPT/swt-01/issues)**:

```markdown
**Type**: 🆕 Edge Case Discovery  
**Description**: App crashes with large inputs  

**Steps**:  
1. Enter `999999 * 999999`  
2. Press `=`  

**Observed Behavior**:  
- Blank screen  
- Console error: `RangeError`  

**Suggested Priority**: Medium  

# 🆕 New Bug Discovery

**Feature Area**: Multiplication Logic  
**Discovered During**: REQ-XX test case: 1.2 * 2.5

**Description:** Multiplication involving decimal numbers also returns an incorrect result.

## 📋 Reproduction Steps  
1. Enter: `1.2 * 2.5`  
2. Press: `=`  
3. Observe result

**Expected:** 3
**Actual Output:** -1.3

## Recommendation  
- Fix the `calculate()` function to correctly evaluate expressions using `eval()` or proper parsing.

## Console Logs  
- No console error, logic fails silently
