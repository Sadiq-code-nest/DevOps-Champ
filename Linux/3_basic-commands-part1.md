- ls
    
    Shows files and folders in the current directory.
    
- ll
    
    Shows detailed info (permissions, size, owner, date).
    
- ls -a
    
    List all files, including hidden ones
    
- ls -l
    
    Long format list with file permissions and metadata
    
- ls -ah
    
    Show all files (including hidden) in human-readable size
    
- mkdir
    
    Make a new directory (folder)
    
    ```bash
    mkdir devops
    # To create multiple folders
    mkdir folder1 folder2
    
    ```
    
- pwd
    
    Print current working directory
    
- touch file.txt
    
    Create an empty file (or update its timestamp)
    
    ```bash
    touch notes.txt
    ```
    
- rm
    
    Remove (delete) a file
    
    ```bash
    rm file.txt
    # Permanently deletes. No recycle bin!
    ```
    
- rm -r
    
    Remove a directory recursively
    
    ```bash
    rm -r foldername
    #  Use this to delete folders and their inner contents.
    ```
    
- rmdir
    
    Remove empty directory
    
    ```bash
    rmdir devops
    # Will fail if the directory is not empty.
    ```
    
- head
    
    View the first 10 lines of a file.  Use `head -n 3` to show first 3 lines.
    
    ```bash
    head sample.txt
    # Use head -n 5 to show first 5 lines.
    ```
    
- tail
    
    View the last 10 lines of a file
    
    ```bash
    tail log.txt
    # Use tail -n 20 for last 20 lines.
    ```
    
- tail -f
    
    **Follow file changes in real-time**
    
    ```bash
    tail -f /var/log/syslog
    #Used to monitor live logs.
    # Analogy: Like watching a WhatsApp group where new messages appear live.
    ```
    
- cd ..
    
    **Move up one directory level**
    
    ```bash
    cd ../../
    # Use multiple .. to go higher:
    ```
    
- echo
    
    Prints a string to the terminal
    
    ```bash
    echo Hello World
    # Great for displaying variables or simple outputs.
    ```
    
- echo “anything” > file.txt
    
    Create or overwrite a file with text
    
    ```bash
    echo "Welcome to DevOps" > intro.txt
    
    # Overwrites the file content. Use >> to append instead
    echo "Next line" >> intro.txt
    
    ```
    
- cat
    
    Display file contents
    
    ```bash
    cat notes.txt
    #  Can also combine files:
    cat file1.txt file2.txt > combined.txt
    
    ```
    
- zcat
    
    ```bash
    # Read contents of compressed .gz files without extracting
    zcat logs.gz
    ```
    
- more
    
    **View file page-by-page (forward only)**
    
    ```bash
    more bigfile.txt
    #  Press spacebar to go down, q to quit.
    ```
    
- less
Better viewer than `more` (supports forward & backward scroll)
    
    ```bash
    less bigfile.txt
    
    🧠 Press ↑ ↓, /pattern, n, q to navigate.
    📦 Tip: Use less for large log or config files.
    ```