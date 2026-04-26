# Phase 1: Requirements and Use Cases

## 1. Actors
- Admin
- Operator

---

## 2. Main Use Cases
- Add Item (Vehicle)
- Search Item
- Issue Item (Rent Vehicle)
- Return Item
- View Transaction History
- Check Availability

---

## 3. Detailed Use Cases

### Use Case 1: Add Item
- Actor: Admin
- Description: Admin adds a new item (vehicle) to the system.
- Precondition: Admin is accessing the system.
- Main Flow:
  1. Admin enters item details (name, type, availability)
  2. System validates input
  3. Item is added successfully
- Failure Case:
  - Missing or invalid details → system shows error

---

### Use Case 2: Issue Item (Rent Vehicle)
- Actor: Operator
- Description: Operator rents an available item to a user.
- Precondition: Item must be available
- Main Flow:
  1. Operator selects item
  2. Operator enters customer details
  3. System checks availability
  4. System records transaction
  5. Item availability is updated
- Failure Case:
  - Item not available → operation rejected

---

### Use Case 3: Return Item
- Actor: Operator
- Description: Operator returns an issued item.
- Precondition: Item must be currently rented
- Main Flow:
  1. Operator selects rented item
  2. System updates availability
  3. System records return transaction
- Failure Case:
  - Invalid return request → system shows error

---

### Use Case 4: View Transaction History
- Actor: Admin
- Description: Admin views all past transactions.
- Precondition: Records exist
- Main Flow:
  1. Admin opens records panel
  2. System displays all transactions
- Failure Case:
  - No records available → show empty message

---

## 4. Acceptance Criteria

### For Issue Item:
- System must prevent issuing unavailable items
- System must update availability after issue
- Transaction must be recorded

### For Return Item:
- System must update availability after return
- Return must be recorded in history

### For Add Item:
- System must validate input
- Item must be added successfully

---

## 5. Main Workflow Focus
Add Item → Issue Item → Return Item → View Records
