ITYOURWAY - Project One

Overview
This project focuses on troubleshooting a deployment issue, managing file permissions, user and group administration, and automating user onboarding using a shell script. It consists of three main tasks:
- Fixing a Deployment Issue & File Management
- User & Group Management
- Automating User Onboarding with a Script

Task 1: Fixing a Deployment Issue & File Management
1. Verify the Deployment Path
Check if the deployment script is using the correct file path.

If the path is incorrect, identify the correct location of the file and inform the developers.

2. Create and Modify a Text File
Create a new file in the home directory and add a specific sentence to it.
Replace the placeholder group number with your actual group number.
Verify the file's group ownership.
Check the file’s permissions to see what access others have.

3. Adjust File Permissions
Change the file permissions to grant full access to the owner, read and write access to the group, and no access to others.
Change the ownership of the file to a specific user.

4. Create a Directory and Set Up Links
Navigate to the /opt directory and create a new subdirectory.
Inside this directory, create a symbolic (soft) link to the file.
Also, create a hard link to the same file in the directory.

5. Compare Inode Numbers
Examine the inode numbers of the original file, the soft link, and the hard link.
Identify the differences between the inode numbers of each type of link.

6. Extract the Root Username
Use a command to extract and display only the username of the root user from the system's password file.

7. Modify sudoers for a Specific Group
Add a group to the system’s sudoers file to allow its members to execute commands with administrative privileges.
Configure the group to be able to run sudo commands without requiring a password.


Task 2: User & Group Management
1. Verify and Create a Group
Check whether a specific group already exists on the system.
If the group does not exist, create it with a predefined group ID.

2. Create a New User
Add a new user with a given username.
Assign the user to the newly created group.
Set the user's full name and default shell.

3. Assign Sudo Privileges
Modify the system configuration to grant sudo access to the group.
Ensure that all members of the group automatically receive sudo privileges.

4. Allow Passwordless Sudo Access
Modify the sudoers file to allow the group members to execute sudo commands without entering a password.

5. Verify User Access
Switch to the newly created user.
Confirm the username by running a command.
Retrieve user details, including group memberships.
Check which sudo commands the user is permitted to run.


Task 3: Automating User Setup
1. Automate Group Creation
Write a script that checks if the required group exists.
If the group does not exist, create it with a specified group ID.

2. Automate User Creation
Ensure the script checks for an existing user before creating a new one.
Assign the user to the designated group.

3. Grant Sudo Privileges
Automatically modify the sudoers file to give administrative rights to the group.

4. Enable Passwordless Sudo Access
Configure the sudoers file to allow members of the group to execute commands without requiring a password.

5. Verify User Setup Automatically
In the script, switch to the newly created user.
Execute commands to confirm the username, group memberships, and available sudo privileges.

6. Run the Script
Set execution permissions on the script.
Execute the script as an administrator to set up the user and group automatically.

Conclusion:
This project provides hands-on experience with troubleshooting deployment issues, managing file permissions, creating users and groups, and automating system administration tasks. By implementing these steps, system administration becomes more efficient, secure, and repeatable.


