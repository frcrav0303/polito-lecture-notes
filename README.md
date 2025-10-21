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

## Snippets

These are my personal LaTeX snippets, created for faster note writing.
I won't share them, I used the VS Code extension **HyperSnips** to make them.
