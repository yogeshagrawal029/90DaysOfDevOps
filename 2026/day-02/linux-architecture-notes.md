The core components of Linux (kernel, user space, init/systemd)
  Ans: Kernel: It is the heart of the linux OS which is used to interact with hardware(CPU, Memory, devices).
       user space: The space where user application and program works or run.
       systemd: It is the very 1st process which starts once the linux boots, PID-1 or init process. It means system is the         process which is running in the background which is known as d

How processes are created and managed?
  Ans: 

What systemd does and why it matters?
  Ans: It is the first process started by the kernel (PID 1).
  Responsibilities:
    1. Bootstraps the system (starts services during boot)
    2. Manages background services (daemons)
    3. Handles logging, networking, and device management
  Replaces older init systems like SysVinit.
  Uses unit files to define and control services.

useful folders
/ - top most directory, base of the entire file system, every thing starts here
/home - Contains user directories, Each user has their own folder - user
/bin - Contains essential user commands (binaries) - basic commands
/sbin - Contains system/admin commands - system commands
/etc - Contains configuration files - configs
/mnt - Used to temporarily mount filesystems
/tmp - Used for temporary files - temporary 
/usr - Contains user programs and utilities - applications
/var - Variable data (changes frequently) - logs data
/root - Home directory of root user
/dev - Contains device files
/proc - Shows process and system info (virtual filesystem)
/boot - Contains bootloader & kernel files
/lib - System libraries required by /bin and /sbin

Various commands:
1.echo - to print the output
2.pwd - to check the current directory path
3.cd - to get into the folder or directory
4.cat - to check the content of the file
5.ls - to list all the files and folder available(if used with -lrth for long list with reverse with sort and in human         readable)
6.df -h - to check for the disk space usage in human readable form for entire filesystem
7.du -sh - to check the disk space usage for particular folder or directory
8.mkdir - to create the new folder or directory(if used with -p then it will check for the folder present and if not present then it    will create the folder)
9.free -m - to check the memory utilization and free space
10.vi/vim/nano - to write in to the file, it is an editor(i - to insret, :wq - to quit)
11.grep - to search for the pattern or text inside the file
12.top/htop - to monitor system process and resouce usage in realtime
13.ps -ef - to display info about the current running process(e- show all processes on the system, f- detailed form)
14.rm -rf - delete the file or folder in particular directory(r - recersively, f- forcefully, note donot use rm -rf / or rm -rf *)
15.touch - to create an empty file
16.head - to display from the start of the file for first 10 line(-n 2 to view the first 2 row)
17.tail - to display from the end of the file for last 10 lines(-n 2 to view the last 2 rows)
18.clear - to clear the terminal screen
19.apt-get install - Install new package
20.apt-get update - Update existing packages (safe)
21.apt-get upgrade - Update + remove/replace obsolete packages
22.ip -a - to check and manage n/w config(-a - show all n/w interface)
23.telnet - to connect to a remote system or port
24.ping - to check network connection b/w 2 system( -t - how many hops a packet can travel)
25.dig - to Advanced details for DNS queries
26.netstat -tunlp - Shows network connections and listening ports(-t → TCP, -u → UDP, -n → Numeric (no DNS lookup), -l → Listening       ports, -p → Process ID/program name)
27.ss -tunlp - ss is preferred in newer systems, Shows network connections and listening ports(-t → TCP, -u → UDP, -n → Numeric (no       DNS lookup), -l → Listening ports, -p → Process ID/program name)
28.nslookup - to Queries DNS to find IP address from domain
29.curl - to transfer data / test web endpoints
30.wget - to download files from internet
31.hostname - to show or set system name
32.uname -r - to check the kernel version
33.kill - to kill the process(-9 - forcefully)
34.nohup - to run the script in background
35.wc -l - to have no. of lines in the file as count
36.& - to run command in background
37.| - to combine multiple commands
38.&& - it is in operator

Task:
  create folder - mkdir -p yogesh; goto the folder - cd yogesh; create the file - touch yogesh.txt; write into the file - echo "hello   dosto!" > yogesh.txt; view the content in the file - cat yogesh.txt; edit the file - vim yogesh.txt; show again content of            yogesh.txt - cat yogesh.txt; to check first 10 rows then - head yogesh.txt; to check last 10 rows then - tail yogesh.txt
