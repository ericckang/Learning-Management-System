# How to Compile and Run the Project

If you are using localhost in the Client socket:

First, check the main method of the Client class. This below line should be in the code:
socket = new Socket("localhost", 4242);

-To compile the Client, go to the terminal and type and enter: javac Client.java

-To compile the Server, go to the terminal and type and enter: javac Server.java

-To run, first run the server by going to the terminal and type and enter: java Server.java
-Then, run the client by going to the terminal and type and enter: java Client.java

If you are connecting to the remote IP address:

First check, the main method of the Client class. This below line should be in the code:
socket = new Socket("128.211.189.172", 4242);


-Do the above steps for compiling

-To run, you only would need to run the client.

-Also, keep in mind that the data in text files of the remote IP are different from the data in text files of the localhost. Also, if it doesn't work then that would mean the server isn't running on Eric's device, but it should be running until May 7. Also, if it still doesn't work, our video demonstration shows the remote connection.

# Descriptions of each Class
Server:

The Server class stores all the data involved with the features such as account usernames and passwords, account type, quiz names, quiz questions, quiz answers, and student grades. The Server also is responsible for sending information to the client that will be displayed on the GUI. The Server handles all the features such as checking if account credentials are correct, creating and taking quizzes, editing quizzes and accounts, grading quizzes, and viewing a graded quiz.

Client:

The Client class displays the GUI which allows for user interaction. The Client class sends information to the Server to tell the Server what to do. For example, if the user clicked the login button, it would send a message to the server so that the server recognizes that the client is trying to log in. The same thing goes for if the user is trying to do things like edit accounts/quizzes, take/create quizzes, etc. The client also sends data that allows the server to do things. For example, when for user authentication, the client sends the username and password to the server. Another example is for when a user is making a quiz, the client sends the quiz name, question names, and answer names to the server so the server is able to create the quiz.
