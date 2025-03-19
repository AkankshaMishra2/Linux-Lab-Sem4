# Lab 1 & 2: File and Directory Management in Linux

## Objective
Practice creating files and directories using the Linux command line.

## Commands Used

### Creating Multiple Files
Use `touch` with brace expansion:
```bash
touch song{1..6}.mp3 snap{1..6}.jpg film{1..6}.avi
```
This creates:
- `song1.mp3` to `song6.mp3`
- `snap1.jpg` to `snap6.jpg`
- `film1.avi` to `film6.avi`

### Creating Multiple Directories
Use `mkdir`:
```bash
mkdir friends family work
```
This creates the directories `friends`, `family`, and `work`.

## Verifying the Creation of Files and Directories
List the created files and directories:
```bash
ls
```
Expected output:
```
friends  family  work  song1.mp3  song2.mp3  song3.mp3  song4.mp3  song5.mp3  song6.mp3  snap1.jpg  snap2.jpg  snap3.jpg  snap4.jpg  snap5.jpg  snap6.jpg  film1.avi  film2.avi  film3.avi  film4.avi  film5.avi  film6.avi
```

### Screenshots
#### 1. Running the `touch` and `mkdir` commands:
![Creating Files and Directories](screenshots/create_files_dirs.png)

#### 2. Listing the created files and directories:
![Listing Files](screenshots/list_files.png)

## Conclusion
In this lab, we created multiple files using `touch` with brace expansion and multiple directories using `mkdir`, demonstrating efficient file and directory management in Linux.