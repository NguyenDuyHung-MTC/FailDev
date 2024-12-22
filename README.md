# FailDev
Handle system errors or bugs that developers encounter when coding

## 1. Error installing npm without setting permissions
   - **Problem**: Once the user has installed Nodejs, they check the version of npm with npm -v, the following error message will be displayed :
  ```javascript  
  The file C:\Program Files\nodejs\npm.ps1 is not digitally signed. You cannot run this script on the current system. For more information about running scripts and setting execution policy, see about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170
  ```
  - **Solution**: Open terminal and type the command
  ```javascript
  Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
  ```
