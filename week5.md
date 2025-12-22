WEEK 5 – Inter-Process Communication (IPC)
ipes

Named Pipes (FIFO)

Signals

File-based IPC (basit script ile)

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 20 32 20" src="https://github.com/user-attachments/assets/c92b1da0-d03d-4096-9ec1-02b045b1825d" />
<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 20 33 35" src="https://github.com/user-attachments/assets/7d6318ed-3c04-4f21-9591-f5970ee11dea" />
This command demonstrates unnamed pipes, where the output of one process is passed directly as input to another process using the pipe (|) operator.


<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 21 10 45" src="https://github.com/user-attachments/assets/3b73943a-b835-4a53-a636-d90bb3cc6c32" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 21 12 13" src="https://github.com/user-attachments/assets/b087fa2f-eeb6-486e-aef0-3976c1852de9" />


<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 21 12 32" src="https://github.com/user-attachments/assets/e0244126-6d2b-48eb-833b-22fd432fc2aa" />
“Each new terminal session starts in the home directory, so I manually navigated back to the working directory using cd.”

Week 5 – Inter-Process Communication (IPC)

In this week, I explored Inter-Process Communication (IPC) using named pipes (FIFO) in Linux. 
I created a new user and performed all IPC tasks using this user to demonstrate multi-user process interaction.

I created a working directory and a named pipe using the `mkfifo` command. 
Named pipes require two processes: one for writing and one for reading. 
When I executed `cat mypipe`, the terminal waited for input, which is expected behavior because FIFO blocks until another process writes data.

In a second terminal session, I navigated back to the same directory and wrote data into the pipe using `echo`. 
Once the data was written, the reading process immediately received and displayed the message.

This experiment helped me understand blocking behavior, process synchronization, and how Linux handles IPC mechanisms safely and efficiently.











