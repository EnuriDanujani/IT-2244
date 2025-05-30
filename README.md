# IT-2244
OS Practicle


Basic Sleep and Exit This program starts, prints a message, sleeps for 3 seconds, and then exits using exit(0).
Since there is no fork(), it runs as a single process.


Parent-Child Process with Waiting The parent creates a child process using fork().
The child sleeps for 2 seconds and then exits

The parent waits for the child to finish (wait(&status)).

After the child exits, the parent prints the child's exit status using WEXITSTATUS(status).
![449327884-a2f0acba-a223-4767-89c3-ada53197e2b4](https://github.com/user-attachments/assets/f59dec56-9f91-4696-b22d-0baa38dee5a4)

Parent Creating Two Children The parent creates two child processes.
First child sleeps for 1 second, Second child sleeps for 3 seconds.

The parent waits for both children using waitpid().

Once both children exit, the parent prints that both have finished.

![449328012-63931b59-63d7-4f38-8fd5-9758c9e634bd](https://github.com/user-attachments/assets/bcee175e-6824-4c8a-a50e-ab8cffb1c78f)

Tracking Which Child Finishes First The first child sleeps 2 seconds, then exits with status 2.
The second child sleeps 1 second, then exits with status 1.

The parent waits twice, checking which child finishes first.

It prints PID and exit status of both children.
![449328167-370d093a-81a1-4759-a056-5e74d01f103d](https://github.com/user-attachments/assets/f2862f08-685c-4780-8098-74e22484763c)




![449328167-370d093a-81a1-4759-a056-5e74d01f103d](https://github.com/user-attachments/assets/385492b8-1f04-4d76-ae64-bdc84b7cc2df)


Parent, Child, and Grandchild Process The parent creates a child, and the child creates a grandchild.
Grandchild sleeps 2 seconds, exits with status 2.

Child waits for grandchild to finish, prints the exit status, and exits with status 55.

Parent waits for the child, prints the child's exit status, and exits.


![449328295-7fa14afc-b5b9-4fab-9f64-27efeebf816b](https://github.com/user-attachments/assets/d8b9d639-afee-476c-bf80-fee03dda2b3f)

