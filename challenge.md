# Lab 06 Challenge: Install It Yourself

## Question 1
Install the program htop, run it, and write one thing it shows.

Answer: htop shows the live CPU usage, the memory usage and the list of running processes with their PID, user and CPU/memory use.

Command: sudo apt install -y htop, then htop (quit with q)

## Question 2
Which version of apache2 does Ubuntu offer? (Do not install it.)

Answer: 2.4.66-2ubuntu2.6

Command: apt show apache2 | head -4

## Question 3
How many packages are installed on your server now?

Answer: 734 packages

Command: apt list --installed | wc -l

## Question 4
Use Docker to run the tiny Linux image alpine so that it prints Hello from Alpine.

Answer: The alpine container ran and printed Hello from Alpine.

Command: sudo docker run --rm alpine echo "Hello from Alpine"

## Question 5
What is the full path of Docker's key file, and of Docker's sources file?

Answer:
Docker's key file: /etc/apt/keyrings/docker.asc
Docker's sources file: /etc/apt/sources.list.d/docker.sources

Command: ls -l /etc/apt/keyrings/ and ls /etc/apt/sources.list.d/

## Question 6
Remove htop and prove that it is gone.

Answer: htop was removed with apt. After running hash -r, the htop command says "Command 'htop' not found", which proves it is gone.

Command: sudo apt remove -y htop, then hash -r, then htop
