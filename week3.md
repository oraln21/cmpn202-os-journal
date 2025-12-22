Week 3 – File and Directory Management

In Week 3, I focused on understanding Linux file system navigation and basic file and directory management commands.  
I created a dedicated working directory (`week3_test`) to clearly separate this week's tasks from previous weeks.

I practiced navigating the file system using commands such as `pwd`, `cd`, and `ls`, and learned how Linux organises files and directories.  
I also worked with file creation, copying, moving, and deletion commands, which are essential for managing data efficiently in a Linux environment.

This week helped me build confidence in working directly from the terminal and understanding how the Linux file system operates at a practical level.


<img width="2880" height="1800" alt="week3" src="https://github.com/user-attachments/assets/61775445-783e-4679-a83c-cf64a3a781e8" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 38 37" src="https://github.com/user-attachments/assets/513e84d9-6450-4889-9ace-b0e563fa7237" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 40 49" src="https://github.com/user-attachments/assets/24928851-8be2-4370-8402-4455f1c0720e" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 43 06" src="https://github.com/user-attachments/assets/10db5bf1-45f5-4c82-b1b5-c597e7851c19" />

System identification and hardware verification (Ubuntu 25.10 ARM64 on UTM)
This week I verified the identity and core hardware details of my Ubuntu installation running in a UTM virtual machine. I first created a dedicated working directory (~/week3_test) to keep evidence and outputs organised and reproducible. Using pwd, I confirmed the active working path to ensure all subsequent commands were executed in the correct context.

To confirm the operating system and kernel environment, I used:

lsb_release -a to verify the Ubuntu distribution version and codename (e.g., Ubuntu 25.10 “questing”).

uname -a to capture the running kernel version, architecture (aarch64), and build information.

hostnamectl to confirm the system hostname and OS metadata presented by systemd.

I then inspected CPU and architecture details to confirm the ARM64 environment and understand how the VM presents hardware to the guest OS:

lscpu provided a structured summary of CPU architecture, cores, and virtualization-related information.

cat /proc/cpuinfo (sampled with head) showed low-level CPU identification information exposed by the kernel.

These checks are important for system administration and troubleshooting because many performance, compatibility, and package decisions depend on kernel version and CPU architecture. Documenting these outputs also provides evidence that the environment matches the coursework requirements (Ubuntu on ARM64, installed via virtualization).



<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 47 54" src="https://github.com/user-attachments/assets/39528155-63c3-46dd-b269-a871de4a17fa" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 49 54" src="https://github.com/user-attachments/assets/c80fe76f-c491-4bfc-a7e4-d7b79e76af39" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 50 51" src="https://github.com/user-attachments/assets/25839983-50f2-49d8-a2ef-02c206d53e19" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 51 28" src="https://github.com/user-attachments/assets/93bb0cbe-ab86-4157-b8a5-3b712eb40ebb" />

Week 3 – Process Management and System Monitoring

In Week 3, I explored how Linux manages running processes and how system resources are monitored in real time. I started by creating a dedicated working directory for this week and verified my location using the `pwd` command.

I used the `ps` command to display active processes associated with the current terminal session. To gain a complete overview of all running processes and system services, I executed `ps aux`, which provided detailed information such as process IDs (PID), CPU usage, memory consumption, and command names.

To observe system activity dynamically, I used the `top` command. This allowed me to monitor CPU usage, memory usage, load averages, and active processes in real time. This helped me understand how system resources are allocated and how processes compete for CPU and memory.

Additionally, I searched for a specific running process using `ps aux | grep firefox`. This demonstrated how processes can be filtered and identified by name. I also learned that each running process is uniquely identified by a Process ID (PID), which is essential for managing and controlling processes.

Overall, this week improved my understanding of Linux process management and system monitoring tools, which are fundamental concepts in operating systems.



<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 20 04 18" src="https://github.com/user-attachments/assets/7ebed612-e3f0-436b-afda-92ff332070a9" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 19 33 03" src="https://github.com/user-attachments/assets/3ab3f5e5-873f-44f0-9db6-8eb1e471c1ae" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 20 05 07" src="https://github.com/user-attachments/assets/39f2ea66-2007-4ab7-9eea-7cd23d07632f" />


<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 20 06 25" src="https://github.com/user-attachments/assets/038e6e44-ab40-45a1-8723-1743520ee1b5" />

<img width="2880" height="1800" alt="Screenshot 2025-12-22 at 20 07 55" src="https://github.com/user-attachments/assets/769e99af-2af1-4201-b03f-679d52949bbf" />
















