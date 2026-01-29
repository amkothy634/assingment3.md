Assignment 3: User Management and Permissions
Task 1: Create Tupu User
I created the user tupu using the interactive adduser command.
* Command: sudo adduser tupu
* I successfully set the password and filled in the basic user information.
Task 2: Create Lupu User
I created the user lupu with a specific home directory and shell.
* Command: sudo useradd -m -d /home/lupu -s /bin/bash -U lupu
* Troubleshooting: I initially encountered an error because the group 'lupu' did not exist.
*  I solved this by using the -U flag to create the group automatically.
Task 3: Create Hupu System User
I created a system account for hupu that cannot be used for logging in.
* Command: sudo useradd --system --shell /bin/false hupu
Task 4: Granting Administrative (Sudo) Access
I granted sudo privileges to both tupu and lupu so they can perform administrative tasks.
* Commands: * sudo usermod -aG sudo tupu
* sudo usermod -aG sudo lupu
* Troubleshooting: I encountered a "Command not found" error because of a typo (sudu). I corrected this by using the proper sudo spelling.
Task 5: Creating the Project Directory
I created a shared directory for project work.
* Command: sudo mkdir /opt/projekti
AI Disclosure
I used AI to help me understand terminal error messages (specifically the "sudu" typo and "group does not exist" errors)
 and to help structure this Markdown documentation according to the assignment requirements.
