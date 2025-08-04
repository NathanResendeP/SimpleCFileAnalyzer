# 🚀 Simple CLI File Analyzer (C) - C Programming studies with Cybersecurity Focus

## Project Overview

This project is a **simple command-line utility written in C** that allows users to analyze text files. It was developed as a practical exercise to deepen my understanding of **C programming** and its fundamental concepts, with a perspective geared towards **cybersecurity**.

## ✨ Features

The program offers two main functionalities:

1.  **Line Count (`-c <file>`):** Calculates and displays the total number of lines in a specified text file.
2.  **Word Search (`-s <file> <word>`):** Searches for and counts all occurrences of a specific word within a text file.

## 🎯 Cybersecurity Relevance

While this is an introductory project, it addresses concepts crucial to the cybersecurity field:

* **Command-Line Argument Handling (`argc`, `argv`):** Understanding how programs process command-line inputs is the first step towards identifying and exploiting vulnerabilities like command injection or buffer overflows (which will be explored in future projects).
* **Low-Level File Reading and Manipulation (`FILE` I/O):** Many attacks and malware analysis tools involve reading and modifying files at a fundamental level.
* **Memory Control:** The C language offers direct control over memory, which is essential for comprehending how exploits operate and how to write more secure code.
* **Foundation for Tools:** The foundation built here is vital for developing port scanners, forensic analysis tools, and other more complex security utilities.

## 🛠️ Technologies Used

* **Language:** C
* **Compiler:** GCC (GNU Compiler Collection)
* **Development Environment:** Kali Linux, Visual Studio Code

## ⚙️ How to Compile and Run

Follow the steps below to compile and run the program in your Linux environment.

1.  **Clone the Repository (or download the `main.c` file):**
    ```bash
    git clone https://github.com/NathanResendeP/SimpleCFileAnalyzer.git
    cd YourRepoName
    ```
    
2.  **Create an Example Text File:**
    Create a file named `example.txt` (or any other name) with some content for testing:
    ```
    This is the first line.
    Here is the second line.
    The third line has a repeated word: word.
    And one more word.
    ```

3.  **Compile the Code:**
    In your terminal, inside the project folder:
    ```bash
    gcc main.c -o cli_utility
    ```
    This will create an executable file named `cli_utility`.

4.  **Run the Program:**

    * **Count Lines:**
        ```bash
        ./cli_utility -c example.txt
        ```
        Expected output:
        ```
        Counting the lines in the file 'example.txt'

        Total of lines: X
        ```

    * **Search Word:**
        ```bash
        ./cli_utility -s example.txt example
        ```
        Expected output:
        ```
        Searching the word 'example' in the file 'example.txt'

        The word 'example' was found X times.

        ```

    * **Testing Errors (Invalid Arguments):**
        ```bash
        ./cli_utility
        ```
        ```bash
        ./cli_utility -c
        ```
        ```bash
        ./cli_utility -s example.txt
        ```
        These commands should display the program's correct usage message.

## 🤝 Contributions

This project was developed as part of a learning journey. Suggestions and improvements are welcome! Feel free to open an *issue* or submit a *pull request*.

## 👨‍💻 Author

* **Nathan Resende da Silva Pinto** - (https://www.linkedin.com/in/nathan-resende)

---
