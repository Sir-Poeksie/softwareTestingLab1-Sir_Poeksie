# 🐞 Bug Report TEMPLATE
**Copy-paste this when creating new [issues](https://github.com/PLP-Database-DEPT/swt-01/issues)**:
**Type**: 🆕 Edge Case Discovery  
**Description**: App crashes with large inputs  

**Steps**:  
1. Enter `999999 * 999999`  
2. Press `=`  

**Observed Behavior**:  
- Blank screen  
- Console error: `RangeError`  

**Suggested Priority**: Medium  

___________________________________
# Failed Test Report

**Requirement ID**: REQ-45  
**Feature Area**: Addition  
**Test Case**: 2 + 2
 

**Expected Result:** `4`
**Expected**: `5`  
**Actual**: `1`  
**Repro Rate**: 100% 
**Severity**: High  
**Evidence**:
[Bug Screenshot](/UI_Version.png)


**Investigation Notes:**  
- Addition results are always off by +1
- Chrome v125, Windows 11

**Requirement ID**: REQ-XX  
**Feature Area**: Multiplication  
**Test Case**: 3 * 2

## ✅ Steps to Reproduce

1. Launch `calculator.html`  
2. Input: `3 * 2`  
3. Press `=`  

## 🔍 Expected Result  
6

## 🐞 Actual Result  
1

## 📈 Reproducibility  
100%

## 🚨 Severity  
Critical

## 🧾 Notes  
- Multiplication incorrectly performs subtraction
