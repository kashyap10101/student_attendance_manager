# Project Statement: Student Attendance Manager

##  Problem Statement
In educational settings, the traditional method of recording and managing daily student attendance (often using physical registers or simple spreadsheets) is highly susceptible to **human error**, is **time-consuming**, and makes real-time summarization difficult. There is a clear need for a simple, digital, and reliable system to efficiently log student presence and quickly provide accurate cumulative attendance data. [cite_start]This project addresses the problem of **manual inefficiency and data delay** in attendance tracking by designing a technical solution[cite: 11].

---

## Scope of the Project
[cite_start]The scope defines the boundaries and limitations of the current implementation[cite: 100].

### Inclusions (What the project does)
* **Student Enrollment:** The system allows for the one-time registration of students.
* **Cumulative Tracking:** The project tracks attendance based on the total number of days a student is marked **Present**, rather than specific dates.
* **Data Persistence:** Attendance records are reliably saved to, and loaded from, a local JSON file (`attendance.json`).
* **Simple Reporting:** Provides an immediate summary view of all students and their total attendance count.

### Exclusions (What the project does NOT do)
* The system **does not** track specific dates or times of attendance.
* It **does not** include user authentication (login/password).
* It **does not** feature a Graphical User Interface (GUI), relying solely on a Command-Line Interface (CLI).
* It **does not** calculate attendance percentages, projections, or advanced analytics.

---

##  Target Users
[cite_start]The primary end-users for this application are individuals responsible for recording and monitoring student presence in a classroom setting[cite: 102]:

* **Instructors/Teachers:** To quickly record and verify attendance at the beginning of a lecture.
* **Teaching Assistants (TAs):** To manage and submit attendance data to the main course faculty.
* **Small Group Tutors:** For tracking presence in workshops or lab sessions.

---

##  High-Level Features
[cite_start]These are the foundational capabilities of the system, designed to directly address the problem statement[cite: 103]:

1.  **Student Registration:** The ability to add new student names to the attendance dictionary/database.
2.  **Attendance Logging:** Functionality to mark a student as present for a session, which increments their cumulative presence count.
3.  **Data Serialization:** Efficient use of JSON file I/O to ensure records are preserved across multiple uses of the application.
4.  **Summary Display:** Provides a clear, human-readable output of all tracked students and their associated attendance counts.
