# Smart Car Parking System

## Overview
The **Smart Car Parking System** is a C-based application utilizing linked lists for dynamic parking management. It supports vehicle registration, parking space allocation, membership benefits, and revenue tracking. The system efficiently handles sorting and searching functionalities for optimal parking lot utilization.

## Features
- **Vehicle Registration:**
  - Store vehicle number, owner name, arrival/departure time, and parking history.
  - Maintain and update membership details dynamically.
- **Parking Space Management:**
  - Allocate parking spaces based on membership type using linked lists.
  - Update the status of parking spaces upon vehicle entry and exit.
- **Sorting Functions:**
  - Sort vehicles based on parking frequency and total amount paid.
  - Sort parking spaces based on occupancy and revenue generated.
- **Membership Policy:**
  - **Premium Membership:** Users with 100+ total parking hours.
  - **Golden Membership:** Users with 200+ total parking hours.
- **Payment System:**
  - Base charge: Rs 100 for the first 3 hours.
  - Additional charge: Rs 50 per extra hour.
  - 10% discount for members.

## Allocation Policy
- **Golden members:** Allocated parking spaces 1-10.
- **Premium members:** Allocated parking spaces 11-20.
- **Non-members:** Allocated spaces beyond 20 based on availability.

## Data Structures Used
- **Singly Linked List:** Used to manage parking spaces dynamically.
- **Singly Linked List:** Used to store and retrieve vehicle records efficiently.
- **Merge Sort:** Implemented for sorting vehicles based on parking frequency and total amount paid.
- **Bubble Sort:** Used for sorting parking spaces based on occupancy and revenue generated.
- **File Handling:** Used for storing and retrieving parking lot and vehicle data persistently.

## File Handling
- Reads and writes parking space and vehicle data from files (`parking-lot-data.txt`, `complete-vehicle-database-100.txt`).
- Ensures data persistence and retrieval across program executions.

## Installation & Usage
### Prerequisites
- C compiler (MinGW/GCC recommended)
- Makefile support for compilation

### Compilation
```sh
make
```

### Running the Program
```sh
./smart_parking
```

## Usage Instructions
1. **Vehicle Entry:**
   - Enter the vehicle number.
   - If a new vehicle, register with owner name and arrival details.
   - Allocate a parking slot based on membership.
2. **Vehicle Exit:**
   - Enter the parking ID to retrieve vehicle details.
   - Calculate parking duration, update membership, and process payment.
   - Free the parking space.
3. **Display Data:**
   - View current parking lot status and vehicle details.
4. **Sorting Operations:**
   - Sort vehicles based on frequency and amount paid.
   - Sort parking spaces based on revenue and occupancy.

## Future Enhancements
- GUI for better visualization.
- Real-time sensor-based parking detection system.
- Database integration for more efficient data handling.

## License
This project is licensed under the MIT License.

