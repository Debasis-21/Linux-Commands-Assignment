# Linux Commands Assignment – Technical Documentation

## Objective

This document demonstrates practical usage of basic Linux command-line utilities for file handling, content inspection, text searching, file compression, downloading files, modifying permissions, and managing environment variables.

**1. Creating and Renaming Files/Directories**

***Commands:***
```
mkdir test_dir
cd test_dir
touch example.txt
mv example.txt renamed_example.txt
```
***Explanation:***

* mkdir test_dir: Creates a new directory named test_dir.

* cd test_dir: Navigates into the test_dir directory.

* touch example.txt: Creates an empty file named example.txt.

* mv example.txt renamed_example.txt: Renames the file to renamed_example.txt.

This operation is useful when organizing files and structuring project directories.

**2. Viewing File Contents**

***a. Display entire file:***

****Command****
```
cat /etc/passwd
```
* Shows complete contents of the /etc/passwd file, which stores user account details.

***b. Display the first 5 lines:***

****Command****
```
head -n 5 /etc/passwd
```
* Useful for previewing the beginning of a large file.

***c. Display the last 5 lines:***

****Command****
```
tail -n 5 /etc/passwd
```
* Helpful when looking at recently added entries.

***3. Searching for Patterns in Files***

***Command:***
```
grep "root" /etc/passwd
```
***Explanation:***

* grep is used to search for patterns in a file.

* In this example, it searches for occurrences of the string “root” within /etc/passwd.

* This is commonly used for locating specific user or configuration entries.

**4. Zipping and Unzipping Files**

***a. Compress directory:***

****Command****
```
zip -r test_dir.zip test_dir
```
***b. Unzip into a new directory:***

****Command****
```
unzip test_dir.zip -d unzipped_dir
```
***Explanation:***

* zip -r compresses the test_dir directory and its contents recursively into a .zip file.

* unzip -d extracts the zip file contents into unzipped_dir.

These operations are useful for backup, sharing, and archiving.

**5. Downloading Files Using wget**

***Command:***
```
wget https://example.com/sample.txt
```
***Explanation:***

* wget is a command-line utility to download files from the internet.

* Replace the URL with a real file URL to fetch remote content.

**6. Changing File Permissions**

***Command:***
```
touch secure.txt
chmod 444 secure.txt
```
***Explanation:***

* touch creates a file named secure.txt.

* chmod 444 sets the file permission to read-only for all users (owner, group, others).

This is crucial for protecting sensitive files from being modified.

**7. Working with Environment Variables**

***Command:***
```
export MY_VAR="Hello, Linux!"
echo $MY_VAR
```
***Explanation:***

* export assigns a new environment variable named MY_VAR.

* echo $MY_VAR outputs its value.

Environment variables are essential for customizing shell behavior and storing temporary configuration values.

**Final Notes**

* Ensure that screenshots are added for each command to demonstrate execution.

* For the wget example, use an actual URL to show successful download.
