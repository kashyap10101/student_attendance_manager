# Project Statement

## Problem Statement
In educational settings, maintaining accurate and current attendance records is a critical but often time-consuming administrative task. Relying on paper registers or complex spreadsheets can lead to manual errors, inconsistency, and difficulty in quickly summarizing student attendance metrics. The core problem addressed by this project is the **lack of a simple, dedicated, and persistent digital tool** for classroom-level attendance tracking that is easy to use and provides immediate summaries.

## Scope of the Project
This project, **PyAttend**, is scoped to be a **standalone, desktop-based GUI application** that manages and persists student attendance records locally.
1.  Core attendance logging (Present/Absent counts).
2.  Student user management (addition).
3.  Data storage using local JSON files.
4.  Real-time visualization of attendance totals.

## Target Users
The primary target users for the PyAttend application are:
1.  **Educators/Teachers:** Who need a fast, simple way to log attendance for a class during a session.
2.  **Teaching Assistants (TAs):** Responsible for maintaining daily records in labs or tutorials.
3.  **Students (as personal tools):** For tracking their own project hours or small group participation.

## High-Level Features
The system provides the following capabilities:
1.  **Student Registration (Add):** Allows the user to quickly input and register a new student name.
2.  **Session Marking (Mark):** Provides a simple interface to select a student and increment either their **Present** count or **Absent** count.
3.  **Data Visualization (View):** Displays the complete, up-to-date attendance summary for all registered students in an easy-to-read table.
4.  **Persistent Storage (Save/Load):** Manages the entire data set, ensuring records are saved to disk before closing and loaded accurately upon startup.
