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
![445537038-8ffa389f-9913-4af9-a58a-b537e683b705](https://github.com/user-attachments/assets/7d4ac029-5276-4417-a787-faab299a7145)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![445537402-5e5dc0f2-a29f-4b24-9ee9-3a25661f8f5b](https://github.com/user-attachments/assets/d30d3d95-bb74-4c02-8107-147e8b622dfb)

type nul > MyFile.txt

![445537622-2631b0d7-4097-42ca-a458-26c6c14beeca](https://github.com/user-attachments/assets/7fb3875f-7594-47a6-99c3-9bf75e115e97)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![445537975-b25822df-2c90-4536-89eb-61f8f1605bc7](https://github.com/user-attachments/assets/4966758c-4496-43aa-9f0b-368483af4af3)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![445538376-66518138-c815-4b5e-959f-6f11767f8c81](https://github.com/user-attachments/assets/06ca4653-e120-45af-99e8-30da5999c987)

copy MyFile.txt %userprofile%\Desktop\Backup

![445538710-6a2bbe63-a162-4b3f-bc16-c4db32990913](https://github.com/user-attachments/assets/6c6a7bf3-fc2c-48d2-bb47-5b52611fac19)

Move the "MyLab" directory to the "Documents" folder.



## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
```
move MyLab Documents



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

![445539787-88c92570-9e7a-4f51-b1f5-5d5e2484581a](https://github.com/user-attachments/assets/1723db8d-719d-443f-bd46-909c4f37aa94)

## command
```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```

## OUTPUT

![445540054-439426dc-40b4-4df0-b607-61c6f0b4f8dd](https://github.com/user-attachments/assets/bc29aa26-5900-4f1f-beef-762ab52479cc)






# RESULT:
The commands/batch files are executed successfully.

