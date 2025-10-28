What I Learned This Week

This week, we explored various methods of Inter-Process Communication (IPC) in Linux. We practiced with basic pipes, named pipes (FIFOs), signals, and file-based IPC. These methods are essential for enabling communication and data sharing between running processes in an operating system.

Tasks Performed
1. Standard Pipe

We used the | operator to connect two commands. For example:

ls -l | grep .txt

This command lists only .txt files in the current directory.

Screenshot included showing command and output.

2. Named Pipe (FIFO)

We created a FIFO special file using mkfifo, and communicated between two terminals:

mkfifo mypipe
echo "Hello from Nilay" > mypipe
cat < mypipe
Screenshots included for FIFO creation and usage.

3. Signals

We simulated a background process using sleep, then terminated it using kill:

sleep 1000
ps aux | grep sleep
kill -9 [PID]
This taught us how to interact with processes through signals.
Screenshots included showing process and signal usage.

4. File-Based Communication

Two processes interacted via a shared text file:

echo "Data from process 1" > sharedfile.txt
cat sharedfile.txt

Screenshot included showing file write and read.

Conclusion

IPC is a powerful concept that helps build communication between processes in a system. Understanding pipes, signals, and file-based messaging lays the groundwork for advanced system programming and performance optimization.

Named Pipe (FIFO) IPC Demonstration

In this task, I implemented Inter-Process Communication using Named Pipes (FIFOs). This mechanism allows two independent processes to exchange data via a named pipe file.

Steps:

I created a FIFO file using:
mkfifo mypipe
in the first terminal, I sent a message:
echo "Hello from process 1" > mypipe

In a second terminal, I received the message:
cat < mypipe

Message successfully received:
Hello from process 1
See screenshot below for terminal output.

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 13 55 05" src="https://github.com/user-attachments/assets/74f44571-e423-4625-acf0-b336e44e041f" />


<img width="1440" height="900" alt="Screenshot 2025-10-28 at 13 35 18" src="https://github.com/user-attachments/assets/dbe8cd97-5817-443b-9653-724a101f2106" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 13 38 08" src="https://github.com/user-attachments/assets/0a505624-e635-486c-bd70-906c8e967f16" />


<img width="1440" height="900" alt="Screenshot 2025-10-28 at 13 38 59" src="https://github.com/user-attachments/assets/a5e08c28-af21-4e5b-8717-c4241fa320dd" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 13 39 36" src="https://github.com/user-attachments/assets/d263a6b3-b109-4b6e-91b1-596e6a8927bb" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 13 48 41" src="https://github.com/user-attachments/assets/93780c53-214f-4ebf-beda-590d0cf5428f" />














