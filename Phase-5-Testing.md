# Phase 5: Testing, Build, and Demo

## 1. Testing Approach

The system was tested manually by executing different workflows through the GUI to ensure correct behavior and data consistency.

---

## 2. Test Cases

### Test Case 1: Add Vehicle
- Input: Valid vehicle details
- Expected Output: Vehicle added successfully
- Result: Passed

### Test Case 2: Rent Vehicle
- Input: Available vehicle and customer details
- Expected Output: Vehicle is rented and marked unavailable
- Result: Passed

### Test Case 3: Return Vehicle
- Input: Previously rented vehicle
- Expected Output: Vehicle availability updated and record stored
- Result: Passed

### Test Case 4: Prevent Invalid Rent
- Input: Attempt to rent unavailable vehicle
- Expected Output: Operation rejected with error message
- Result: Passed

### Test Case 5: Input Validation
- Input: Missing or invalid customer details
- Expected Output: Error shown and operation blocked
- Result: Passed

---

## 3. Build Process

Compile the project using:

```bash
javac Main/*.java Gui/*.java Service/*.java Model/*.java Util/*.java
