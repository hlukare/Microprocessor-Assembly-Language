# Microprocessor-Assembly-Language

How to run an assembly language program on both Windows and Linux systems using NASM (Netwide Assembler), along with links to install NASM on each platform.
Windows:
Installing NASM:
Download NASM:
Go to the NASM website: NASM - The Netwide Assembler (https://www.nasm.us/)
Click on the "Download" section.
Choose the appropriate installer for your Windows version (32-bit or 64-bit).

Install NASM:
Run the downloaded installer.
Follow the installation instructions.
Ensure that NASM is added to your system PATH during installation.
Running Assembly Language Program:
Write Your Assembly Code:
Use a text editor like Notepad or any code editor of your choice to write your assembly code. Save the file with a .asm extension, for example, my_program.asm.

Assemble Your Code:
Open Command Prompt (cmd) or PowerShell.
Navigate to the directory where your assembly file is located using the cd command.
Run the following command to assemble your code: nasm -f win32 my_program.asm -o my_program.obj
This command will generate an object file (my_program.obj) from your assembly code.

Link Your Object File:
Use a linker like ld or gcc to link your object file. For example, using gcc: gcc my_program.obj -o my_program.exe

Run Your Program:
Execute your compiled program by typing its name in the command prompt: my_program.exe












Linux:
Installing NASM:
Install NASM using Package Manager:
Open Terminal.
Run the following command: sudo apt-get install nasm
Enter your password when prompted.
Running Assembly Language Program:
Write Your Assembly Code:
Use a text editor like Vim, Nano, or any code editor of your choice to write your assembly code. Save the file with a .asm extension, for example, my_program.asm.

Assemble Your Code:
Open Terminal.
Navigate to the directory where your assembly file is located using the cd command.
Run the following command to assemble your code: nasm -f elf64 my_program.asm -o my_program.o
nasm -f elf64 my_program.asm -o my_program.o
This command will generate an object file (my_program.o) from your assembly code.

Link Your Object File:
Use a linker like ld or gcc to link your object file. For example, using gcc: gcc my_program.o -o my_program

Run Your Program:
Execute your compiled program by typing its name in the terminal: ./my_program
