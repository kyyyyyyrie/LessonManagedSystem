# LessonManagedSystem

A Java-based course management system with a Swing GUI interface.

## Features

- **Course Management**: Add, delete, and update course information
- **Search Functionality**: Search courses by any field (course name, ID, type, grade, or teacher)
- **Filter Options**: Filter courses by grade level and course type
- **Data Persistence**: Course data stored in text files for persistence

## Technology Stack

- Java
- Swing (GUI framework)

## Project Structure

```
src/
  |- Main.java              # Application entry point
  |- edu/
     |- neuq/
        |- Class/
        |  |- start.java    # Main controller, handles data loading/saving
        |  |- Lesson.java   # Course data model
        |  |- Cla.java      # Individual course entity
        |- Handler/
        |  |- MainAction.java    # Main menu action handler
        |  |- MainAction01.java  # Type filter handler
        |  |- MainAction02.java  # Grade filter handler
        |  |- addAction.java    # Add course handler
        |  |- delAction.java    # Delete course handler
        |  |- updateAction.java # Update course handler
        |- UI/
           |- MainMenu.java   # Main application window
           |- addMenu.java    # Add course dialog
           |- delMenu.java    # Delete course dialog
           |- updateMenu.java # Update course dialog
data/
  |- name.txt      # Course names
  |- ID.txt        # Course IDs
  |- type.txt      # Course types (required/elective)
  |- grade.txt     # Grade levels
  |- teacher.txt   # Teacher names
```

## Course Fields

- Course Name
- Course ID
- Course Type (Required / Elective)
- Grade Level (Freshman / Sophomore / Junior / Senior)
- Teacher Name

## How to Run

1. Ensure Java is installed
2. Compile the source files:
   ```
   javac -d out src/*.java src/edu/neuq/**/*.java
   ```
3. Run the application:
   ```
   java -cp out Main
   ```

## Usage

1. Launch the application to view the main course list
2. Use "Add" button to add new courses
3. Use "Delete" button to remove courses
4. Use "Update" button to edit existing course information
5. Use "Search" button to search for specific courses
6. Use the dropdown filters to filter by grade or course type
7. Click "Exit" to save and exit