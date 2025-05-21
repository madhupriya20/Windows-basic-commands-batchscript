# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "my-folder"

## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\MyLab
```
![alt text](445537038-8ffa389f-9913-4af9-a58a-b537e683b705.png)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```

![alt text](445537402-5e5dc0f2-a29f-4b24-9ee9-3a25661f8f5b.png)

type nul > MyFile.txt

![alt text](445537622-2631b0d7-4097-42ca-a458-26c6c14beeca.png)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![alt text](445537975-b25822df-2c90-4536-89eb-61f8f1605bc7.png)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![alt text](445538376-66518138-c815-4b5e-959f-6f11767f8c81.png)

copy MyFile.txt %userprofile%\Desktop\Backup

![alt text](445538710-6a2bbe63-a162-4b3f-bc16-c4db32990913.png)

Move the "MyLab" directory to the "Documents" folder.



## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
move MyLab Documents

![alt text](445539218-6329267a-e08b-4990-be54-1cb3d7e7dfa0.png)

## Exercise 2: Advanced Batch Scripting
Create a batch file named on the desktop. The batch file need to have a variable assigned with a desired name for ex. name="John" and display as "Hello, John".
## command
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

## OUTPUT

![alt text](445539787-88c92570-9e7a-4f51-b1f5-5d5e2484581a.png)

## command
```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```

## OUTPUT



![alt text](445540054-439426dc-40b4-4df0-b607-61c6f0b4f8dd.png)




# RESULT:
The commands/batch files are executed successfully.

