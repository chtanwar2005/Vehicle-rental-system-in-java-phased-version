# Phase 3: Database and DAO Layer

## 1. Database Design

The system uses a structured data model similar to a relational database. Although file-based storage is used, the design follows database principles.

### Tables

#### Vehicle (Item)
- id (Primary Key)
- name
- type
- available

#### Customer (User)
- id (Primary Key)
- name
- phone

#### Rental (StockEntry)
- rentalId (Primary Key)
- vehicleId (Foreign Key)
- customerId (Foreign Key)
- days

#### RentalRecord (Transaction)
- recordId (Primary Key)
- vehicleId (Foreign Key)
- customerId (Foreign Key)
- status

---

## 2. DAO Layer Design

The project uses a utility class (FileUtil) to handle data persistence.

This acts similar to a DAO layer by:
- Storing data in files (.dat)
- Reading and writing records
- Supporting CRUD operations

---

## 3. CRUD Operations

### Vehicle
- Create → addVehicle()
- Read → getVehicle()
- Update → update availability
- Delete → remove vehicle (if implemented)

### Rental
- Create → rentVehicle()
- Read → view active rentals
- Update → update rental details
- Delete → returnVehicle()

### Records
- Create → store transaction
- Read → view history

---

## 4. Data Flow

User Action → GUI → Service Layer → FileUtil → Data Storage

---

## 5. Justification

Although JDBC is not used, the system follows DAO principles by separating data handling logic from business logic.

File-based storage is used to simulate database operations, making the system simpler while maintaining proper architecture.


---


## 6. Implementation Reference

The FileUtil class is used as the data persistence layer and simulates DAO operations.
