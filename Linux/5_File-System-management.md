- ssh
    
    Securely connect to a remote Linux server
    
- df
    
    Check disk space usage of file systems
    
- df -h
    
    Disk space usage in human-readable format (MB, GB)
    
- du .
    
    Check space used by the current directory
    
- ps
    
    View running processes
    
- top
    
    **Live process monitor. Real-time CPU, memory usage, and running processes — like Task Manager in Windows.**
    
- htop
    
    ### (Better version of `top`)
    
    **Interactive and colorful process monitor.** 
    Easier to read, allows you to **kill processes directly**.
    
- fuser
    
    Find which process is using a file or port
    
    ```bash
    fuser -v /var/log/syslog
    fuser -n tcp 8080
    # Useful for detecting why a file or port is busy.
    ```
    
- kill -9
    
    Forcefully kill a process by PID
    
    ```bash
    kill -9 1234
    ```
    
- free -h
    
    Check memory (RAM) usage in human-readable format
    
- nohup
    
    Run a command that survives terminal logout.
    
    ```bash
    nohup python3 [script.py](http://script.py/) &
    
    # -------------------------
    Prevents the command from stopping if you close the terminal.
    📁 Output goes to nohup.out file by default.
    ```
    
- vmstat
    
    Report virtual memory, CPU, and I/O stats
    
    ```bash
    vmstat 2 5
    # Shows system performance every 2 seconds, 5 times.
    ```