# Login Test
Steps:

1. User launches application.
2. User clicks Login button.
3. User enters username via the keyboard.
4. User enters password via the keyboard.

Expected result: Application verifies the user's username and password and loads their homepage automatically. 
For example, if the entered username was teach and the entered password was pass, the teacher page should load.
If the entered username was stu and the entered password was pass, the student page should load.

Test Status: Passed. 

# Create Account Test
Steps:

1. User launches application.
2. User clicks Create Account button.
3. User enters username via the keyboard.
4. User enters password via the keyboard.
5. User selected account type via the dropdown menu.

Expected result: Application creates the account and the relevant files (passwords.txt users.txt and accountTypes.txt) are updated with the entered data

Test Status: Passed. 

# Create Course Test
Steps:

1. User launches application and logs in with a teacher account.
2. User clicks Create Course button.
3. User enters the new course name via the keyboard.

Expected result: Application creates the course and the relevant file (courses.txt) is updated with the entered data

Test Status: Passed. 

# Create Quiz Test
Steps:

1. User launches application and logs in with a teacher account.
2. User clicks Access Courses button.
3. User selects a course via the dropdown menu.
4. User selects the add quiz option.
5. User enters title of quiz via the keyboard.
6. User enters number of questions for the quiz via keyboard.
7. User enters number of answers per question via keyboard.
8. User enters in the name of question.
9. User enters in the answer options.
10. After they are done, a success message should pop up.

Expected result: Application creates the quiz and the relevant file (listOfQuizzes.txt and '(quiznamegoeshere)'answers.txt and '(quiznamegoeshere)'questions.txt) is updated with the entered data

Test Status: Passed. 

# Take Quiz Test
Steps:

1. User launches application and logs in with a student account.
2. User clicks Access Courses button.
3. User selects course via dropdown menu.
4. User selects quiz via dropdown menu.
5. User selects answers via dropdown. The program should display the question and then have a dropdown of the associated answer options for that question.
6. Once finished, program goes back to student page.

Expected result: Application creates timestamped file of the students answers with all of their selected answers.

Test Status: Passed. 

# Edit Quiz Title Test
Steps:

1. User launches application and logs in with a teacher account.
2. User clicks Access Courses button.
3. User selects course via dropdown menu.
4. User selects edit quiz option via dropdown menu.
5. User selects quiz via dropdown.
6. User selects edit quiz title option via dropdown.
7. Once finished, program goes back to teacher page.

Expected result: Application updates listOfQuizzes.txt with the new quiz name and updates the answers and questions file with the new quiz name.

Test Status: Passed. 

# Edit Quiz Question  Test
Steps:

1. User launches application and logs in with a teacher account.
2. User clicks Access Courses button.
3. User selects course via dropdown menu.
4. User selects edit quiz option via dropdown menu.
5. User selects quiz via dropdown.
6. User selects edit quiz question option via dropdown.
7. User selects what question to change via dropdown.
8. User enters new question.
9. Once finished, program goes back to teacher page.

Expected result: Application updates the questions file with the new quiz question.

Test Status: Passed. 

# Edit Quiz Answer  Test
Steps:

1. User launches application and logs in with a teacher account.
2. User clicks Access Courses button.
3. User selects course via dropdown menu.
4. User selects edit quiz option via dropdown menu.
5. User selects quiz via dropdown.
6. User selects edit quiz answer option via dropdown.
7. User selects what answer to change via dropdown.
8. User enters new answer.
9. Once finished, program goes back to teacher page.

Expected result: Application updates the answers file with the new answer.

Test Status: Passed. 

# Concurrency Test

1. User launches application twice by running the client twice.
2. User logs in with two accounts.
3. If concurrency works, there should be no issues with logging in.
4. Once logging in works, users should be able to do things with the buttons like creating courses or accessing courses without interference.
5. Exit the program and check to see if there was any interference/conflict.

Expected result: No interference or conflicts occur when running multiple clients. Everything functions as normal.

Test Status: Passed. 
