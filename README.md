# Student Attendance Manager

## 🌟 Overview of the Project
This project is a simple **Command-Line Interface (CLI)** application developed in **Python** for managing and tracking student attendance. It allows the user to add students, mark their daily attendance (incrementing a count), and view a summary of the total days present for each student. All attendance data is automatically persisted in a local **JSON file** (`attendance.json`) between application runs.

### Project Alignment
[cite_start]This project aligns with the course objectives by demonstrating the application of core programming concepts, data structures (dictionaries), modular programming, and data persistence (file I/O)[cite: 5, 8].

## ✨ Features
[cite_start]This system implements the following core functional modules[cite: 21]:

* **1. Student Enrollment:** Allows the user to add a new student to the system (`add_student()` function).
* **2. Attendance Marking:** Allows the user to mark a specific student as present, which increments their cumulative attendance count (`mark_attendance()` function).
* **3. Attendance Summary:** Displays a complete list of all students and their total days present (`view_summary()` function).
* **4. Data Persistence:** Handles loading the attendance data on startup and saving it to the `attendance.json` file upon exit (`save_data()` function).

## 💻 Technologies/Tools Used
* **Primary Language:** Python 3.x
* **Libraries/Modules:** `json` and `os` (standard, built-in modules)
* [cite_start]**Version Control:** Git (Required for tracking implementation changes) [cite: 55]

## ⚙️ Steps to Install & Run the Project

### Prerequisites
* Ensure **Python 3.x** is installed on your operating system.

### Installation
1.  **Clone the Repository:**
    ```bash
    git clone [YOUR_REPOSITORY_URL]
    cd [YOUR_PROJECT_FOLDER]
    ```
2.  No external libraries or packages are required.

### Running the Application
1.  Execute the main Python script from your terminal:
    ```bash
    python main_attendance.py  # Assuming your file is named main_attendance.py
    ```
2.  The application will present a menu. Select options (1-4) to interact with the system.

## ✅ Instructions for Testing

Testing is performed by interacting with the CLI menu to verify data manipulation and persistence.

1.  **Start the Program** (Run the script).
2.  **Test Case 1: Add and Mark Present**
    * Select **1. Add Student** and enter a name (e.g., "Alice").
    * Select **2. Mark Attendance** and mark "Alice" as present ('y').
    * Select **3. View Attendance Summary** and confirm that "Alice: 1 days present" is displayed.
3.  **Test Case 2: Mark Absent and Persistence**
    * Select **2. Mark Attendance** and mark "Alice" as absent ('n'). The count should remain 1.
    * Select **4. Save & Exit**.
4.  **Test Case 3: Data Integrity**
    * **Re-run** the program.
    * Select **3. View Attendance Summary** and confirm that the count for "Alice" is still correctly loaded as 1, demonstrating reliable persistence.
