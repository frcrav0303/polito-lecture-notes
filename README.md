# Lecture Notes, PoliTO 2025

A collection of my university lecture notes written in LaTeX.
I write my notes using LaTeX on VSCode, with a personal template and custom snippets inspired by the late Gilles Castel.

These are **personal notes**, which means they may be incomplete or contain inaccuracies.
Do not take them as professional or official material.

## Folder Structure

- `/course_name/` — Contains all notes for a specific course
  - `main.tex` — Main LaTeX file
  - `lectures/` — Individual lecture files
  - `info.yaml` — Course metadata
  - `out/main.pdf` — Compiled output

To build the course structure, I use a Python3 script that I wrote myself. It prompts me to enter parameters such as **COURSETITLE** and **SEMESTER**, which are then automatically inserted into both the `info.yaml` and `main.tex` files.

I then made the script executable on macOS, and by running the command:
```makecourse course-name```

I also made a script to create and manage individual lectures inside the current course directory.
Unlike the makecourse script, which builds the overall course structure, makelecture focuses on handling lecture-level operations.
It has some new features, like:

- Create a new lecture file inside the `../lectures/` dir.
- Automatically update the main.tex file by adding the new input lecture line.
- Remove an existing lecture (and its reference in main.tex)
- List all the already existing lecture files in the `../lectures/` directory

For example: ```makelecture --remove lec_02``` will remove the "lec_02.tex" file.

I also added a logging feature, which automatically creates a log file to keep track of all lecture operations — such as creations and deletions.
All logs are stored in the `logs/` directory, allowing me to easily review the history of changes across courses.

## Snippets

These are my personal LaTeX snippets, created for faster note writing.
I won't share them, I used the VS Code extension **HyperSnips** to make them.

## Acknowledgements

Thank you for taking the time to explore my lecture notes.
I hope you find them useful and inspiring for your own studies.
Any feedback, suggestions, or contributions are always welcome!
