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

## Data Manipulation
### 1. grep
Purpose:
Searches for matching patterns in a file.
Use case:
Used to identify TP53 mutations in a mutation dataset.
Example:
grep TP53 mutations.tsv

### 2. wc
Purpose:
Counts lines, words, or characters.
Use case:
Used to count the number of mutation records.
Example:
grep TP53 mutations.tsv | wc -l

### 3. head
Purpose:
Displays the first lines of a file.
Use case:
Used to inspect the beginning of annotation or sequence files.
Example:
head annotations.gtf

### 4. tail
Purpose:
Displays the last lines of a file
Use case:
Used to inspect the end of data files.
Example:
tail annotations.gtf

## Git and GitHub
### 1. git add
Purpose:
Stages changes before committing.
Use case:
Used to prepare updated documentation or scripts for version control.
Example:
git add .

### 2. git commit
Purpose:
Creates a snapshot of project changes.
Use case:
Used to record progress during bioinformatics analysis.
Example:
git commit -m "Added data analysis notes"

### 3. git push
Purpose:
Uploads committed changes to GitHub.
Use case:
Used to synchronize local changes with the remote repository.
Example:
git push

### 4. Commit Messages
Purpose:
Provide descriptive records of project changes.
Use case:
Used to document meaningful project progression.

## Text Processing and File Operations
### 1. cut
Purpose:
Extracts specific columns from structured files.
Use case:
Used to extract mutation type or genomic coordinates from tabular data.
Example:
cut -f 2 mutations.tsv

### 2. sort
Purpose:
Sorts lines in a file.
Use case:
Used to order mutation records or genomic coordinates.
Example:
sort mutations.tsv

### 3. uniq
Purpose:
Identifies or counts unique values.
Use case:
Used to count mutation categories.
Example:
sort mutations.tsv | uniq -c

### 4. join
Purpose:
Merges two files using a common field.
Use case:
Used to combine related biological datasets.

## Key Learnings
Through this course I developed foundational understanding of:

- Linux command-line navigation

- Shell tools for handling biological data

- Pattern searching and data manipulation

- Git and GitHub for reproducible research

- Text processing tools used in bioinformatics workflows
