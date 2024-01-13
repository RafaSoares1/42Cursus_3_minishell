# Minishell

## About

Welcome to the realm of shells with MiniShell, your gateway to the world of text-based interfaces that empower you to interact effortlessly with your operating system.<br />
This was without any doubt the most challenging project so far, because Shell encompass distinct and well-defined behaviors in nearly every scenario, demanding careful handling.
Made together with [ZPedro99](https://github.com/ZPedro99).

⚠️***This is Minishell and not Bash 2.0, it is possible to find small errors in the project***⚠️

## Little Demo On How The Project Works

![ezgif com-video-to-gif](https://github.com/RafaSoares1/42Cursus_3_minishell/assets/103336451/28a81b0a-5da0-4c5a-b92f-7b5bf87cea95)

## Main Goal

This project was a significant milestone for me, representing both the most extensive undertaking and my initial experience working collaboratively within a group.<br />
The primary objective revolved around developing a compact version of a bash shell, which, despite being labeled "mini," proved to be a huge project.<br />
Throughout the process, we delved into understanding how bash handles arguments, parsing them effectively, and executing the corresponding commands. The incorporation of the following features further enhanced the complexity of the project:

* Implement a prompt: ensuring users can input commands comfortably while awaiting new instructions
* Working history: enabling users to access and execute previously entered commands efficiently
* Robust Execution: We incorporated the ability to find and launch executables, using the PATH variable or absolute paths to ensure the command execution
* Quote Handling: Managed single and double quotes, like in bash
* Redirection Support: Our implementation embraced various redirections, including input (<), output (>), heredoc (<<), and append mode (>>)
* Pipe Functionality: We empowered the interpreter with the capability to handle pipes (|)
* Environment Variables: enabling users to interact with and manipulate their environment
* Handle $?: giving the correct exit status
* Handle signals: ctrl-C, ctrl-D, and ctrl-\ should behave like in bash.
* Recreate the following builtins:<br />
        - echo with option -n.<br />
        - cd with only a relative or absolute path.<br />
        - pwd (no flags).<br />
        - export (no flags).<br />
        - unset (no flags).<br />
        - env (no flags or arguments).<br />
        - exit (no flags).<br />

## What is Shell an how does it work?

For the realisation of the project we have used this [guide](https://www.cs.purdue.edu/homes/grr/SystemsProgrammingBook/Book/Chapter5-WritingYourOwnShell.pdf) several times to help us in the construction of our project.<br />
But in a summarised way, the Shell Bash, often referred to simply as Bash, is a Unix shell and command language. It is the default shell for most Linux distributions and macOS systems, and it is also available on various other Unix-based operating systems. Bash stands for "Bourne Again SHell," a pun on "Bourne Shell," which was an earlier Unix shell.<br />

At its core, Bash is a command-line interface that allows users to interact with the operating system through textual commands. It acts as an intermediary between the user and the operating system, accepting user input (commands) and translating them into actions that the operating system can execute.

Here's how Bash works:

1. **Command Interpretation**: When you open a terminal or command prompt and type a command, Bash reads that input and interprets it. The command can be a simple one-liner like "ls" to list files in the current directory or a more complex script with multiple commands and logic.

2. **Parsing and Tokenization**: Bash parses the input command, breaking it down into individual components or tokens. It separates the command and its arguments, identifies special characters like pipes (|) for creating pipelines, input/output redirection symbols (<, >), and other elements that affect how the command is executed.

3. **Command Execution**: After parsing and tokenization, Bash identifies the appropriate command to execute based on the input. If it is a built-in command (e.g., cd for changing directories), Bash handles it directly. If it is an external command (e.g., ls, grep, etc.), Bash searches for the executable binary in the directories listed in the system's PATH variable and then launches the corresponding program.

4. **I/O Redirection and Pipelines**: Bash manages input/output redirection and pipelines. For instance, when you use ">" to redirect the output of a command to a file, or ">>" to append output to a file, Bash handles these operations. Similarly, when you use "|" to connect multiple commands together, forming a pipeline, Bash manages the flow of data between them.

5. **Environment Variables**: Bash allows users to set and access environment variables. These variables store information that can be used by the shell or by programs executed from the shell. Environment variables help configure the shell's behavior and provide useful information like the current working directory (PWD), user information (USER), and more.

6. **Scripting**: Bash is not limited to interactive use; it also supports scripting. Users can write scripts, which are essentially a sequence of commands saved in a file with the ".sh" extension. These scripts can be executed just like any other command, and they enable users to automate tasks and create more complex sequences of actions.

In summary, Bash is a powerful and versatile shell that facilitates interaction with the operating system and allows users to perform a wide range of tasks, from simple command execution to complex scripting and automation. It provides a foundational layer for many system administration tasks, programming, and software development on Unix-based systems.

## Installation

After cloning the repository, the program is compiled into a ***minishell*** executable using:
```sh
make 
```
or
```sh
make all
```
## Final Grade
![Screenshot 2023-08-01 at 13-57-37 Intra Projects minishell](https://github.com/RafaSoares1/42Cursus_3_minishell/assets/103336451/6c3d244e-fa29-4001-8972-0b5a66a0050b)
