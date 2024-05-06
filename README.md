# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```

![328017511-80cb2424-a260-4f56-bfcf-58e533d4497b](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/eb616fec-2beb-4d2f-bc93-03f70b09d22e)


## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab

```

![328017561-9a8501d1-b220-422e-980f-a76bdb5c8396](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/2a6e1f2c-808a-42b6-aa86-459f9f91ad26)
![328017594-9224d7fb-a4fd-4a1e-a1a4-2433722875c1](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/615896a3-ae37-4d51-95c6-0b6f5e952e4a)




## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab

```
![328017769-01529418-e0dc-44ca-90ef-a3ce4ba33578](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/c9c7a2b4-56ce-4679-96d7-75df1e0f0c1b)


## COMMAND AND OUTPUT


Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![328017864-a0dbb303-e603-4a48-b308-ccaeb318e56e](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/3eae30e9-54c3-4e31-b420-6a8e51b09261)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![328017960-eb1d3916-8346-4456-b72f-f8201d23fa16](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/99a40adc-a8ac-4ca3-9d13-e6a595798f5d)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![328018081-524e0614-396d-49f2-8992-0135b4bcf177](https://github.com/Harsetha/Windows-basic-commands-batchscript/assets/149985878/a2785698-1782-44b7-ad1a-3935a21392f1)




# RESULT:
The commands/batch files are executed successfully.

