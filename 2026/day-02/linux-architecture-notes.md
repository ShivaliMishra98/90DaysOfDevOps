## LINUX FUNDAMENTALS
- Linux is an open source operating system, most popular to build apps. Developed by Linus Torvalds. "Eveyrthing in linux is a file or a folder/directory".
- Architecture: ASK = Application, Shell, Kernel --> Users interact with the kernel(which contains the hardware like monitor, printer,ect) via the Shell(black screen) using shell commands. Terminal contains the shell.
- "Everything in linux is a process": Every process starts with init/systemd (system daemon which runs in background) with <mark>PID 1</mark>. systemd is a device manager used to start/stop/restart any services using the systemctl commands.
- When we Power On a device, the BIOS chips the motherboard which loads the hardware --> hardware loads the GNU GRUB which loads the linux kernel --> this is when we see the OS logo loading --> this loads the first process systemd which initiates the hardware, CPU scheduling making it ready to use. 

## PROCESS STATES:
- Running(R) -> When the process is currently using the CPU
- Sleeping(S) -> Inactive state where process is waiting for a signal to wake up or I/O event completion, thereby not utilising the CPU.
- Stopped(T) -> The process has been abruptly terminated/ halted (example pressing Ctrl+Z in terminal). It receives <mark/>SIGSTOP</mark>  signal.
- Zombie(Z) -> Process has completed it's execution but still has en entry in the system process table. When a process dies it sends <mark>SIGCHLD</mark> signal to it's parent. The parent must call <mark>wait()</mark> to read child's exit status. Until the parent does this, the child remains a 'zombie'.

## SHELL COMMANDS:
- cd : change directory
- ls : list 
- man : to view command's description
- pwd : present working directory
- cp src destn : copy from source to destination
- ps aux | grep nginx : active processes running for process nginx
- mkdir (directory name) : create a directory
- touch (file name) : create file
