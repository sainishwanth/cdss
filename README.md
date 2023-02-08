# Compiler Design and System Software Lab

This repository contains all the Python, Prolog, and Lisp programs that I have executed for my Artificial Intelligence Course in my 3rd Year of Computer Science Undergrad program at Dayananda Sagar University, Bengaluru, India in Q1 2023.

## List of Programs

| Serial No. | File Name | Description |
| :---: | :--- | :--- |
| 1a | [1a_CharCount.l](https://github.com/rexgraystone/cdss/blob/main/1a_CharCount.l) | A Lex program that count the number of characters, spaces, words and lines in a given text file. |
| 1b | [1b_IdentifierCount.l](https://github.com/rexgraystone/cdss/blob/main/1b_IdentifierCount.l) | A Lex program that count the number of identifiers in a given program file. |

## How to Run

1. Ensure that you have a C compiler installed on your system.

    ```bash
    gcc --version
    ```

    It should look something like this ![GCC Version](Images/GCC_Version.png "GCC Version")

    If you don't have a C compiler installed, you can download one from [here](https://sourceforge.net/projects/mingw/) or using your package manager.

    Examples:

    - Ubuntu -

    ```bash
    sudo apt install gcc
    ```

    - Arch Linux -

    ```bash
    sudo pacman -S gcc
    ```

    - macOS -

    ```bash
    brew install gcc
    ```

    Additionaly, if you are using Windows, follow the steps specified [here](https://www.scaler.com/topics/c/c-compiler-for-windows/).

2. Clone the repository using the following command:

    ``` bash
    gh repo clone rexgraystone/cdss
    ```

    or

    ``` bash
    git clone https://github.com/rexgraystone/cdss.git
    ```

3. Change the directory to the cloned repository:

    ``` bash
    cd cdss
    ```

**For Lex programs:**

1. Compile the Lex program using the following command:

    ``` bash
    lex <filename>.l
    ```

    Example:

    ``` bash
    lex 1a_CharCount.l
    ```

2. Compile the generated C file using the following command:

    ``` bash
    gcc lex.yy.c -ll -o <Output File Name>
    ```

3. Run the program using the following command:

    ``` bash
    ./<Output File Name>
    ```
