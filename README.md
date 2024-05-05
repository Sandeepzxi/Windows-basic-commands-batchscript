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

mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/81669a4d-ffc2-439a-80c8-1b46e9cb0702)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab
![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/9d733373-ca71-4e34-8a30-5f72533fd170)
![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/0d9c8c90-f227-44b2-b6c0-034a358fb5dc)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/05538d19-0977-4edb-88d6-e3c1d5743746)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
Move the "MyLab" directory to the "Documents" folder.
```
![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/a30ae995-c2a5-4849-a9a9-602bc32186a9)

![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/d46b7de0-9878-401b-9dce-7e94b966e9c9)

## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```


## OUTPUT

![image](https://github.com/Sandeepzxi/Windows-basic-commands-batchscript/assets/168530813/f0d35bfe-c68e-4f19-a3c7-d41834414583)




# RESULT:
The commands/batch files are executed successfully.

