# Badminton-Courts-Booking-App-Mendix

This repository contains the software engineering project for a **Booking Badminton Court Mobile Application**. It was submitted by **Heang Company** for the **ITDS262: Software Engineering** course at the Faculty of ICT, Mahidol University.

The project's goal is to address the growing popularity of badminton and the need for health-conscious activities by providing a convenient, all-in-one digital platform for booking courts and equipment. This application aims to streamline operations for court owners and enhance the booking experience for players.

---

## 1. Key System Features

The application is designed with two primary user roles, each with a dedicated set of functionalities:

### 👩‍💻 For Users (Players)
* **User Management:** Secure registration and login for new and existing users.
* **Court Searching:** Ability to search for courts by name, price, or distance.
* **Geo-location:** Integrates with a Location API to find and recommend nearby courts.
* **Booking System:** Book courts and related equipment for specific dates and times.
* **Online Payments:** Secure payment processing via online banking, including QR code generation.
* **Cancellations:** Ability to cancel a booking and request a refund (e.g., must be 30 minutes prior to the booked time).
* **Feedback:** A satisfaction rating system (5-star) and comment section for users to provide feedback after their session.

### 🔒 For Administrators
* **Court & Equipment Management:** Full CRUD (Create, Read, Update, Delete) capabilities for managing court details, availability, and equipment inventory.
* **User Administration:** Ability to manage user accounts, including suspending users who violate terms.
* **Reporting:** Access to view and analyze customer satisfaction reports and comments.
* **Financials:** Authority to approve refund requests for eligible cancellations and issue tax invoices.

## 2. Software Engineering & Design Artifacts

This repository contains a comprehensive set of design documents from both project phases, detailing the system's architecture and logic.

### Phase 1: Requirements & Conceptual Design
* **Functional & Non-Functional Requirements:** A detailed list specifying system capabilities and constraints, such as supporting 3 languages (Thai, English, Chinese), 1000 concurrent users, and 2-second search processing.
* **Actor Identification:** Defined 5 key actors: **User**, **Administrator**, **Court Officer**, **Bank**, and **Location API**.
* **Use Case Diagram:** A high-level visual model of actor interactions with the system's main functions.
* **Use Case Narratives:** Detailed step-by-step descriptions for key processes, including "Submit Court Booking," "Submit Equipment Booking," and "Submit Rating".

### Phase 2: System & Process Modeling
* **Functional Decomposition Diagram:** A hierarchical chart breaking the main "Badminton Court Booking System" into 7 high-level processes (e.g., Manage Data, Manage User, Search, Book, Payment).
* **Data Flow Diagrams (DFDs):**
    * **Context Diagram (Level 0):** Shows the entire system as a single process interacting with all external entities.
    * **DFD Level 1:** Decomposes the system into its 7 main processes and shows data flows between them and the data stores.
    * **DFD Level 2:** A set of detailed diagrams, one for each of the 7 processes, showing their specific sub-processes and data handling.
* **Data Stores:** The system's architecture is built on 5 core data stores:
    1.  D1: Court and Equipment Database
    2.  D2: User Database
    3.  D3: Court and Equipment Booking Database
    4.  D4: Payment Database
    5.  D5: Satisfaction Rating Database

## 3. Prototyping & Testing

* **Low-Code Prototype (Mendix):** As confirmed in the GitHub repository, the UI/UX mockups for the application were developed using the **Mendix** low-code platform. The prototyped screens include a "Courts Overview" page, a "Court Editing" page, and a "Booking" management page.
* **Test Cases:** The project includes formal test cases for quality assurance, such as the detailed test plan for the "Home page" module.
