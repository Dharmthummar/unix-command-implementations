# OS Practicals Unix

This repository contains practical assignments for an Operating Systems (OS) course, focusing on Unix command implementations and system programming concepts. The programs include shell scripts and C programs that demonstrate fundamental OS functionalities, such as file manipulation, process management, and directory operations, primarily in a Unix-like environment.

## Purpose
The purpose of this repository is to showcase implementations of Unix commands and OS-related utilities developed as part of college practical assignments. These programs illustrate concepts like file I/O, process threading, and command-line utilities, serving as a learning resource for OS students.

## Files and Descriptions
The repository includes the following files, each implementing specific OS-related functionality:

- **cmpfile.sh**: Compares two files and outputs whether their contents are identical. If different, it shows the differences using `cmp`.
- **append.sh**: Concatenates multiple files (or non-file inputs with user confirmation) into a single output file (`concatenated_file.txt`).
- **dbms.sh**: Implements a simple database management system, allowing users to create, display, insert, delete, update, sort, and search records in a text file.
- **revnum.sh**: Reverses a given input number, handling both positive and negative numbers.
- **pthread.c**: A C program demonstrating POSIX threads (pthreads), creating two threads that print messages concurrently.
- **grep.c**: A C program implementing a simplified version of the `grep` command, searching for a string in a file and printing matching lines.
- **end.sh**: Accepts text input until the word "end" is entered, saves it to a file (`destination`), and displays the content with a line count.
- **head.sh**: Mimics the Unix `head` command, displaying the first N lines of a specified file.
- **dirmange.sh**: A directory management script for creating, modifying, navigating, listing, and managing permissions of files and directories.
- **tail.sh**: Mimics the Unix `tail` command, displaying the last N lines of a specified file.

## Prerequisites
To run these programs, you need:
- A Unix-like environment (e.g., Linux, macOS, or WSL on Windows).
- For shell scripts (`.sh`):
  - Bash shell (`bash`).
  - Standard Unix utilities (`cat`, `grep`, `sort`, `wc`, etc.).
- For C programs (`.c`):
  - GCC compiler (`gcc`).
  - POSIX thread library for `pthread.c` (included in most Unix-like systems).
- Basic permissions to execute scripts and create files/directories.

## Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Dharmthummar/unix-command-implementations.git
   cd unix-command-implementations
   ```

2. **Set Execute Permissions for Shell Scripts**:
   ```bash
   chmod +x *.sh
   ```

3. **Compile C Programs**:
   For `pthread.c`:
   ```bash
   gcc -o pthread pthread.c -pthread
   ```
   For `grep.c`:
   ```bash
   gcc -o grep grep.c
   ```

## Usage
Below are example commands to run each program. Ensure you are in the repository directory.

- **cmpfile.sh**:
  ```bash
  ./cmpfile.sh file1.txt file2.txt
  ```
  Compares `file1.txt` and `file2.txt`, showing if they are identical or their differences.

- **append.sh**:
  ```bash
  ./append.sh file1.txt file2.txt
  ```
  Concatenates files to `concatenated_file.txt`. Prompts for non-file inputs if provided.

- **dbms.sh**:
  ```bash
  ./dbms.sh
  ```
  Runs an interactive menu for database operations (create, insert, delete, update, sort, search).

- **revnum.sh**:
  ```bash
  ./revnum.sh
  ```
  Prompts for a number and outputs its reverse (e.g., `123` becomes `321`).

- **pthread.c**:
  ```bash
  ./pthread
  ```
  Runs two threads that print "Thread 1" and "Thread 2" messages.

- **grep.c**:
  ```bash
  ./grep "search_string" filename.txt
  ```
  Prints lines from `filename.txt` containing `search_string`.

- **end.sh**:
  ```bash
  ./end.sh
  ```
  Accepts text input until "end" is entered, saves to `destination`, and shows the line count.

- **head.sh**:
  ```bash
  ./head.sh filename.txt 5
  ```
  Displays the first 5 lines of `filename.txt`.

- **dirmange.sh**:
  ```bash
  ./dirmange.sh
  ```
  Runs an interactive menu for directory/file creation, modification, navigation, and permissions.

- **tail.sh**:
  ```bash
  ./tail.sh filename.txt 5
  ```
  Displays the last 5 lines of `filename.txt`.

## Notes
- **Academic Context**: These programs were developed as part of an Operating Systems course to demonstrate Unix command implementations and system programming concepts.
- **Error Handling**: Some scripts (e.g., `dbms.sh`, `dirmange.sh`) may have typos or logical errors (e.g., `fanme` in `dbms.sh`, `dirmange` instead of `dirmanage`). These are preserved as per the original assignment code but may need debugging for production use.
- **Improvements**: For real-world use, consider adding input validation, error handling, and documentation within the scripts.
- **License**: This project is for educational purposes. Feel free to use, modify, or share under the MIT License (see `LICENSE` file, if added).

## Contributing
This is an academic project, but suggestions for improvements or bug fixes are welcome! Please submit issues or pull requests via GitHub.

## Contact
For questions or feedback, contact Dharm Thummar at dthummar17@gmail.com or open an issue on this repository.
