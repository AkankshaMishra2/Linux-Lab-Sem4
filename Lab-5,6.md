# Lab 5 & 6: Using Vim and Nano to Edit Files in Linux

## Objective
Learn to use **Vim** and **Nano** to edit files in Linux.

## Commands and Concepts

### 1. Setting Up the Lab File
Create the file if it doesn't exist:
```bash
touch editing_final_lab.txt
```
Store the file path in a variable:
```bash
lab_file="editing_final_lab.txt"
```

### 2. Editing with Nano
Open the file in Nano:
```bash
nano $lab_file
```
Add the following text:
```
This is the first line of the file.
This is the second line of the file.
This is the third line of the file.
```
Save (`CTRL + O`) and exit (`CTRL + X`).

### 3. Editing with Vim
Open the file in Vim:
```bash
vim $lab_file
```
Tasks in Vim:
1. Enter visual mode (`v`).
2. Remove the last seven characters of the first line.
3. Preserve only the first four characters of the first line.
4. Save and exit (`:wq`).

### Verifying Command Execution
Check the file contents:
```bash
cat $lab_file
```
Expected output after editing:
```
This
```

## Conclusion
You learned to use **Nano** and **Vim** for file editing in Linux, including basic text manipulation in Vim.