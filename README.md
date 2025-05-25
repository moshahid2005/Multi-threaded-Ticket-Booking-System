This project simulates a multithreaded ticket booking system where multiple users attempt to book seats concurrently. The system uses core Java concurrency tools and demonstrates synchronization, file handling, and clean architecture practices.

Features
Console-based ticket booking interface.

Multithreading to simulate multiple users booking at the same time.

Thread-safe booking operations using synchronized methods or ReentrantLock.

Logs booking information to a file.

Modular structure separating models, services, and UI.

Project Structure
cpp
Copy
Edit
src/
├── model/
│   ├── Ticket.java       // Holds seat and user info
│   └── User.java         // User-related attributes
├── service/
│   └── BookingService.java // Synchronized methods for safe booking
├── ui/
│   └── ConsoleUI.java    // Console-based interaction
│   └── MainApp.java      // Entry point
└── threads/
    └── UserThread.java   // Implements Runnable for user simulation
Setup Instructions
Prerequisites
Java JDK 17 or higher.

IDE: IntelliJ IDEA, Eclipse, or any Java-supporting IDE.
Implementation Details
Shared resource: List<Integer> to manage available seats.

Concurrency control via synchronized methods or ReentrantLock.

Booking data is stored in a .txt or .csv file using java.io.

Safe file I/O through synchronized blocks.

Demo
The application will prompt for:

Number of available seats.

Number of users attempting to book.
It will then simulate each user as a separate thread trying to book a seat and display the results in the console.

License
This project is licensed under the MIT License.

