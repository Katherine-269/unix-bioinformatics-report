# Unix Bioinformatics Report

## Purpose
This repository documents Linux, Unix, Git, and bioinformatics concepts learned during the course.

## Topics Covered
- Linux Essentials
- Shell Expansions
- Data Manipulation
- Git and GitHub
- Text Processing

## Status
Repository under development. Module-wise documentation will be added progressively.

## 1.Linux Essentials

### 1. pwd
Purpose:
Prints the current working directory.
Use case:
Helps identify the current location while navigating biological datasets.

### 2. ls
Purpose:
Lists files and directories in the current location.
Use case:
Used to view available sequence files, datasets, or folders.

### 3. cd
Purpose:
Changes the current directory.
Use case:
Used to move between different data folders in a bioinformatics project.

### 4. mkdir
Purpose:
Creates a new directory.
Use case:
Used to organize data into folders such as raw data, processed data, and results.

### 5. touch
Purpose:
Creates an empty file.
Use case:
Used to create placeholder files such as scripts or notes.

## Shell Expansions and Redirection

### 1. Wildcards (*)
Purpose:
Used to match multiple filenames.
Use case:
Can select multiple FASTA files at once.
Example:
*.fasta

### 2. Pipes (|)
Purpose:
Passes output from one command into another command.
Use case:
Used to filter and count biological features.
Example:
grep TP53 mutations.tsv | wc -l

### 3. Output Redirection (>)
Purpose:
Sends command output into a file.
Use case:
Used to save extracted coordinates or analysis results.
Example:
grep TP53 mutations.tsv > tp53_results.txt
