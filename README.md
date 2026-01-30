# Hospital-Management-System-HMS-

A simple, menu-driven Hospital Management System (HMS) implemented in C. The system manages patients, doctors, and appointments using in-memory data structures (C structs) and core concepts like arrays and functions. This version avoids file I/O to keep things straightforward for learning.

## Features
- Patient management
  - Add new patients
  - Display patient details
  - Search for patients
- Doctor management
  - Add doctors
  - Assign doctor to a patient
- Appointment scheduling
  - Schedule appointments
  - View all appointments
  - Update appointment status
- User-friendly, menu-driven interface
- In-memory data (no file storage)

> Purpose: Educational project to illustrate core C concepts (structs, arrays, functions) in a hospital context.

## Getting Started

### Prerequisites
- A C compiler (e.g., gcc)
- Basic knowledge of C (structs, arrays, pointers, functions)

### How to Run
1. Clone the repository
2. Compile (example with gcc): gcc -o hms main.c./hms
3.  Use the on-screen menu to manage patients, doctors, and appointments.
> If your project uses multiple source files, adjust the command, for example:
gcc -o hms main.c patient.c doctor.c appointment.c

## Data Models (Overview)
- Patient
  - id, name, age, gender, diagnosis
- Doctor
  - id, name, specialization
- Appointment
  - id, patient_id, doctor_id, date (YYYY-MM-DD), time (HH:MM), status

All data is stored in memory (no persistent storage in this version).

## Project Structure (Suggested)
- main.c or app.c – Entry point and menu loop
- patient.c / patient.h – Patient data structures and operations
- doctor.c / doctor.h – Doctor data structures and operations
- appointment.c / appointment.h – Appointment data structures and operations
- utils.c / utils.h – Helper functions (e.g., search, display)
- README.md – This file

> Adapt file names to match your actual project layout.

## Design Goals
- Simplicity: Clear, easy-to-understand code and flow
- Learnability: Demonstrates modeling real-world entities with C structs
- Core functionality: Basic HMS operations without external dependencies

## Limitations
- No file storage or database (data is in-memory for the session)
- Basic error handling appropriate for an educational project
- No concurrency or data persistence across runs

## Future Enhancements (Suggestions)
- Add file I/O to persist data between sessions
- Improve search and reporting features
- Validate inputs more rigorously
- Introduce user roles (admin, receptionist, doctor)
- Add appointment reminders and status transitions

## Testing (Basic Workflow)
- Add a patient and verify a unique ID is assigned
- Add a doctor and verify a unique ID is assigned
- Display patient details
- Search for a patient by ID or name
- Schedule and view appointments
- Update appointment status (e.g., Completed, Cancelled)

## Contributing
Contributions are welcome. If you have ideas to improve functionality or fix bugs:
- Fork the repo
- Create a feature branch
- Commit with clear messages
- Open a pull request

## License
Educational project. (Specify your preferred license, e.g., MIT, Apache-2.0, if desired.)

