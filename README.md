# Capstone2

## Task Description

Follow these steps:
● Use the task_manager.py file, together with the supporting text files user.txt and tasks.txt for this Capstone project. In this task, you will be modifying task_manager.py to extend its functionality. Working on existing code files to extend them is great practice for working in a developer team on an established code base.
● You will notice that the main body of the code requires functionality for registering a user, adding a task, viewing all tasks, and viewing the current user's tasks. However, because there is so much functionality needed to complete this, the main body of the loop becomes difficult to read. Using the principle of abstraction, refactor the code to create and use the following functions:
o reg_user — a function that is called when the user selects ‘r’ to register a user.
o add_task — a function that is called when a user selects ‘a’ to add a new task.
o view_all — a function that is called when users type ‘va’ to view all the tasks listed in ‘tasks.txt’.
o view_mine — a function that is called when users type ‘vm’ to view all the tasks that have been assigned to them.
● Modify the function called reg_user to make sure that you don’t duplicate usernames when you add a new user to user.txt. If a user tries to add a username that already exists in user.txt, provide a relevant error message and allow them to try to add a user with a different username.
● Add the following functionality when the user selects ‘vm’ to view all the tasks assigned to them:
o Display all tasks in a manner that is easy to read. Make sure that each task is displayed with a corresponding number that can be used to identify the task.
o Allow the user to select either a specific task (by entering a number) or input ‘-1’ to return to the main menu.
o If the user selects a specific task, they should be able to choose to either mark the task as complete or edit the task.

If the user chooses to mark a task as complete, the ‘Yes’/’No’ value that describes whether the task has been completed or not should be changed to ‘Yes’.
▪ If the user chooses to edit a task, the username of the person to whom the task is assigned or the due date of the task can be edited. The task can only be edited if it has not yet been completed.
● Add an option to generate reports to the main menu of the application.

When the user chooses to generate reports, two text files, called task_overview.txt and user_overview.txt, should be generated. Both these text files should output data in a user-friendly, easy to read manner.
o task_overview.txt should contain:
▪ The total number of tasks that have been generated and tracked using the task_manager.py.
▪ The total number of completed tasks.
▪ The total number of uncompleted tasks.
▪ The total number of tasks that haven’t been completed and
that are overdue.
▪ The percentage of tasks that are incomplete.
▪ The percentage of tasks that are overdue.
o user_overview.txt should contain:
▪ The total number of users registered with task_manager.py.
▪ The total number of tasks that have been generated and
tracked using task_manager.py.
▪ For each user also describe:
▪ The total number of tasks assigned to that user.
▪ The percentage of the total number of tasks that have
been assigned to that user
▪ The percentage of the tasks assigned to that user that
have been completed
The percentage of the tasks assigned to that user that must still be completed
▪ The percentage of the tasks assigned to that user that has not yet been completed and are overdue
● Modify the menu option that allows the admin to display statistics so that the reports generated are read from tasks.txt and user.txt and displayed on the screen in a user-friendly manner. If these text files don’t exist (because the user hasn’t selected to generate them yet), first call the code to generate the text files.
