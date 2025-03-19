# Lab 7 & 8: Managing Permissions and Directories in Linux

## Objective
Learn to manage directories, set permissions, and configure `umask` for a user.

## Commands and Concepts

### 1. Create the `/home/consultants` Directory
```bash
sudo mkdir /home/consultants
```

### 2. Add Write Permission to the `consultants` Group
```bash
sudo chmod g+w /home/consultants
```

### 3. Forbid Others from Accessing the Directory
```bash
sudo chmod 770 /home/consultants
```

### 4. Verify Permissions
```bash
ls -ld /home/consultants
```
Expected output:
```
drwxrwx--- 2 root consultants 4096 Oct 10 12:34 /home/consultants
```

### 5. Change the Default `umask` for the `operator1` User
1. Switch to `operator1`:
   ```bash
   sudo su - operator1
   ```
2. Set the new `umask`:
   ```bash
   echo "umask 007" >> ~/.bashrc
   source ~/.bashrc
   ```
3. Verify the new `umask`:
   ```bash
   umask
   ```

### 6. Confirm the `umask` is Applied
Create a new file and directory, then check permissions:
```bash
touch testfile
mkdir testdir
ls -l
```
Expected output:
- File: `-rw-rw----`
- Directory: `drwxrwx---`

## Conclusion
You learned to manage directories, set permissions, and configure `umask` in Linux.