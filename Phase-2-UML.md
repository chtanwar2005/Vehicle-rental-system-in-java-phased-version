# Phase 2: UML and Package Design

## 1. Package Structure

The project follows a layered architecture with clear separation of concerns:

- model → contains entity classes such as Vehicle, Customer, Rental, RentalRecord  
- service → contains business logic (RentalService)  
- gui → contains Swing UI classes  
- util → contains utility classes like FileUtil  
- main → contains application entry point  

---

## 2. Core Classes

### Vehicle
Represents an inventory item with attributes like id, name, type, and availability.

### Customer
Represents a user who rents items.

### Rental
Represents an active transaction where a vehicle is issued to a customer.

### RentalRecord
Stores completed transaction history.

### RentalService
Handles business logic such as issuing and returning vehicles and updating availability.

---

## 3. Design Principles

- Separation of concerns between UI, business logic, and data handling  
- Business logic handled in service layer instead of GUI  
- Data persistence handled using FileUtil  
- Classes represent real-world entities  

---

## 4. UML Class Diagram

(See diagram below)
[VehicleRental_UML_ClassDiagram.pdf](https://github.com/user-attachments/files/27135147/VehicleRental_UML_ClassDiagram.pdf)
