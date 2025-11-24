#  Student Attendance Manager

## Project Title
**PyAttend:** A Simple GUI-Based Student Attendance Manager

## Overview of the Project
The PyAttend application is a desktop utility designed to efficiently manage and track student attendance records. Developed using **Python** and the **Tkinter** library for a user-friendly Graphical User Interface (GUI), this tool replaces tedious manual record-keeping with a simple, digital solution. It allows users (like educators or teaching assistants) to add students, mark them as present or absent for a session, and save the cumulative data securely using JSON serialization.

## Key Features (High-Level)
* **CRUD Operations:** Seamlessly **Add** new student records, **Read** (view) the current attendance status, and **Update** (mark present/absent) records.
* **Persistent Storage:** Records are automatically loaded upon startup and saved to a local `attendance.json` file, ensuring data integrity across sessions.
* **Intuitive GUI:** Uses standard Tkinter widgets (Buttons, Combo-boxes, Treeview Table) for easy navigation.
* **Detailed Summary:** Displays a real-time table showing the total count of days a student was marked **Present** and **Absent**.

##  Technologies & Tools Used
* **Primary Language:** Python 3.x
* **GUI Library:** `tkinter` and `tkinter.ttk`
* **Data Persistence:** `json` module for File I/O (JSON serialization/deserialization)
* **Version Control:** Git

##  Steps to Install & Run the Project

This project requires a standard Python 3 environment.

### Prerequisites
1.  Ensure you have **Python 3.x** installed.
2.  Tkinter is typically included with standard Python installations, so no external libraries are usually required.

### Running the Application
1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/kashyap10101/student_attendance_manager
    cd Student_Attendance_Manager
    ```
2.  **Execute the Script:**
    ```bash
    python attendance_manager.py 
    ```
    *Note: The first time you run the script, it will automatically create an empty `attendance.json` file.*

##  Instructions for Testing
To confirm the application is working correctly, follow these basic test cases:

1.  **Data Persistence Test:**
    * Click the **Add** button and add a new student (e.g., "Kashyap").
    * Mark this student **Present** twice using the **Mark** button.
    * Click **Save** or exit the application and choose **Save**.
    * Rerun the script. The table should correctly display "Kashyap" with a Present count of 2.
2.  **Marking Test:**
    * Add a new student (e.g., "Rohit").
    * Use the **Mark** function to mark Rohit **Absent**.
    * The student's entry in the table should show Present: 0 and Absent: 1.
3.  **Error Handling Test:**
    * Attempt to add a student name that already exists (e.g., "Kashyap"). The application should show the **"Already got that one"** warning message and not duplicate the entry.
4.  **Save/Exit Prompt Test:**
    * Make an unsaved change (e.g., mark a student present).
    * Attempt to close the main window using the standard "X" button. The application must prompt you with the **"Save first?"** dialog box.
