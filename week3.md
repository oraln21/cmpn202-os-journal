Activity: System Monitoring and Resource Commands
Objectives:

Practice system monitoring using basic Linux commands.

Compare resource usage in different Linux distributions (Ubuntu + Alpine).

Understand running processes, memory, disk usage, and system performance.
Commands Executed and Outputs:
who
nilay    tty2         2025-10-27 14:16
w
 15:01:57 up  2:46,  1 user,  load average: 0.00, 0.02, 0.00
USER     TTY      FROM             LOGIN@   IDLE   JCPU   PCPU WHAT
nilay    tty2                      14:16    2:46m  0.01s  0.01s /usr/libexec/gnome-session
top
Screenshot Taken 

Load average: Low

CPU usage: ~0%

Memory used: ~1.2GB of 3.3GB

Swap: Not used

Running processes: Mostly root and nilay

Note: Pressing q exits the top command.

ps aux
Output:

Shows processes owned by root and nilay

Some important processes: gnome-shell, python3, bash, nano

lsmod
Output:

Modules like snd, virtio_gpu, ip_tables, usb_storage loaded.

Useful for checking what drivers or services are active.

df -h
Output:

Root partition (/dev/vda2) → 62G total, 9.2G used

/dev/vda1 → EFI partition

/run, /boot/efi, /tmp, and systemd services shown

uname -a
Output:

Linux nilay-QEMU-Virtual-Machine 6.1.0-5-generic #1 SMP PREEMPT_DYNAMIC Mon Sep 22 09:50:31 UTC 2025 aarch64 GNU/Linux

Observations:

Ubuntu is fully operational in the QEMU virtual machine.

Memory usage is low; CPU load is minimal.

No swap memory is currently used.

Essential kernel modules (sound, network, display) are properly loaded.

Screenshots Taken:
who / w command result
top screen output
ps aux process list
lsmod modules list
df -h disk usage
uname -a kernel info

Learning Summary:

In this week, I practiced key system monitoring commands in a Linux environment. I gained confidence in using tools like top, ps, and df to observe how the system operates internally. I also learned how to interpret resource usage, understand user activity, and manage system modules.

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 10 57 37" src="https://github.com/user-attachments/assets/e831f126-5dfb-4835-8ce8-4be50295f32f" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 11 55" src="https://github.com/user-attachments/assets/e41b4149-f6c0-4add-8109-b98552ef62e0" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 50" src="https://github.com/user-attachments/assets/f5b633e7-e886-456c-8929-c6cf33b4e042" />
<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 57" src="https://github.com/user-attachments/assets/3643197d-2433-496a-beeb-811b543b8ed1" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 13 01" src="https://github.com/user-attachments/assets/d7158710-363a-47b8-9711-fd085e2d1d2d" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 13 10" src="https://github.com/user-attachments/assets/65ea7073-0f4f-4a79-a688-e8eeaa8474d4" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 13 53" src="https://github.com/user-attachments/assets/4ba0462a-ca5e-4130-9511-b02586a2dbfc" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 25 31" src="https://github.com/user-attachments/assets/fec6593d-9375-4e5e-9487-2a720c359c90" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 29 59" src="https://github.com/user-attachments/assets/fa62ff01-e23d-46cb-8e9c-81c8b16e312e" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 33 20" src="https://github.com/user-attachments/assets/5ebeaa57-c569-49d1-8e84-65b3d4a8be26" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 33 57" src="https://github.com/user-attachments/assets/bf837372-7056-412a-a37a-cc79fd50fed6" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 35 12" src="https://github.com/user-attachments/assets/b9e7c892-99c4-4d06-b1af-e1f9df463b9b" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 03" src="https://github.com/user-attachments/assets/b68b8703-208e-4169-a87b-7c9591444811" />
<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 14" src="https://github.com/user-attachments/assets/d8c2016d-2d99-4ccc-89fd-7b486a58ff16" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 23" src="https://github.com/user-attachments/assets/5203a5d5-56ed-462a-be9e-6e2f8a93130a" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 29" src="https://github.com/user-attachments/assets/a9efdf53-b871-472b-a100-f42c4d7ae38e" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 39" src="https://github.com/user-attachments/assets/c9efc5f3-e1f8-4b18-8857-f40cbc337f2d" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 12 44" src="https://github.com/user-attachments/assets/47a53b57-ca97-4dc8-9b48-f3c28896c364" />
<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 06 49" src="https://github.com/user-attachments/assets/6011ee64-cd01-4bde-805b-2487aa2ff372" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 07 19" src="https://github.com/user-attachments/assets/3deeda4e-3f89-4b77-bfec-9d951be12589" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 07 39" src="https://github.com/user-attachments/assets/d1f5b25f-594c-426e-8afa-3d73a69c9d95" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 07 39 copy" src="https://github.com/user-attachments/assets/baa35b22-d5a5-454b-a37c-68937971a39b" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 07 52" src="https://github.com/user-attachments/assets/46a83aab-8bbe-43df-bc3f-222fefd74a4f" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 09 55" src="https://github.com/user-attachments/assets/798f19c2-1243-4f90-b0df-99a247618802" />

<img width="1440" height="900" alt="Screenshot 2025-10-28 at 11 10 06" src="https://github.com/user-attachments/assets/c5bd0037-5ab3-45f1-8c64-c3c1552910e1" />




















































