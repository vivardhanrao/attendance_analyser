# attendance_analyser

A Django based application that would be used to display the attendance of students along with necessary graphs. 

There are two modules to the application:

One for students where they can: 
  > See their aggregate attendance.
  > See a pie chart comparing their attendance in all the subjects.
  > Use two handy metrics, one for calculating future attendance and the other for make up attendance.

Other for faculty where they can: 
  > View the attendance of a particular student.
  > View the attendance of a particular subject.
  > View the attendance of a whole class with its respective graph.
  
For the purpose of demonstration we used a sample database (cse.db) that contains: 
> The attendance of students of 2 batches (academic years), where each batch has four sections (A, B, C, D), which correspond to total of 8 tables. 
  Each table consists of one column for roll number (ID) of a student, and other columns for the attendance count in various subjects.
  The first row of each table consists of the total number of classes (till that date) in various subjects (under the ID 'total').
> A table containing the credentials (IDs and passwords) of faculty.

The graphs are generated using 'matplotlib' library ( http://matplotlib.org/ ) in Python.

To run the application on your computer, clone the repository onto your computer and execute command "manage.py runserver" in command line (cmd for Windows). Then go to http://127.0.0.1:8000/ on a browser.
P.S.: Make your current directory as the repository cloned. 

Check 'Demo' directory for screenshots of the project.

Python version: 2.7.12
Django version: 1.10.1
