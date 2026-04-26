# Phase 0: Proposal and Backlog
Project Title

Inventory Management System (Vehicle Rental Based)

Problem Statement

Managing inventory manually often leads to incorrect stock records, poor tracking of item usage, and lack of visibility into availability. In environments where items are frequently issued and returned (like vehicles or equipment), it becomes difficult to track usage history and availability in real time.

This project aims to build a desktop-based inventory management system that allows users to manage items, track their availability, record transactions (issue/return), and maintain a history of usage. The system ensures that stock is updated accurately and prevents invalid operations such as issuing unavailable items.

Target Users
Admin
Manages items (vehicles)
Monitors availability and records
Operator
Issues (rents) items
Returns items
Views current status
Core Entities
Item (Vehicle) → represents inventory items
User (Customer) → person using the item
StockEntry (Rental) → issue/return operation
Transaction (RentalRecord) → history of actions
End-to-End Workflow
Admin adds items (vehicles) to the system
Operator selects an available item
Operator issues (rents) the item to a user
System updates item availability
Operator returns the item
System updates stock and stores transaction history
Admin can view all records and availability
Features Included (Version 1)
Add and manage items
Track item availability
Issue (rent) items
Return items
Store transaction history
Prevent issuing unavailable items
Features Excluded (to control scope)
Billing and payment system
Online/cloud access
Advanced analytics or graphs
Multi-user authentication system
Initial Backlog (Task Breakdown)
High Priority
Add item (vehicle) functionality
Register user (customer)
Issue item (rent vehicle)
Return item
Track availability
Medium Priority
View transaction history
Search items
Low Priority
UI improvements
Error handling and validation
Why This Project Fits the Theme

This project aligns with the Inventory Management System theme because it manages items, tracks stock availability, records transactions, and maintains history. The rental and return process directly maps to stock-out and stock-in operations in inventory systems, making it a suitable real-world implementation of the theme.
