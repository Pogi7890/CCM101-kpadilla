# Laboratory 01 – Welcome to the Cloud

## Mission Overview

Congratulations! I have been accepted as a Junior Cloud Infrastructure Engineer Trainee at CloudNova Technologies.

The first mission focuses on learning how to work inside a Linux environment, document technical work professionally, and maintain a version-controlled portfolio using GitHub.

For this laboratory activity, I used the KillerCoda Playground to access an Ubuntu Linux environment. I explored the Linux system, created a user account, gathered system information, organized files and directories, and prepared my Cloud Computing Portfolio on GitHub.

## Objectives

Upon completing this mission, I should be able to:

- Access a cloud-based Linux environment using KillerCoda.
- Explore and navigate the Linux operating system.
- Gather basic system information.
- Organize files and directories using Linux commands.
- Create and maintain a professional GitHub repository.
- Document technical work using Markdown.
- Demonstrate proper documentation practices used by cloud professionals.

## Activities Performed

1. Accessed the KillerCoda Ubuntu Playground.
2. Verified that the Linux terminal was functioning.
3. Created a personal Linux user account named `kpadilla`.
4. Added the user to the sudo group.
5. Logged in using the new user account.
6. Checked the current username, working directory, and hostname.
7. Gathered information about the Linux distribution, kernel, CPU, memory, and disk space.
8. Created the required directory structure.
9. Created Markdown documentation files.
10. Created a personal Cloud Computing Portfolio.
11. Prepared screenshots as evidence of completed tasks.
12. Initialized the project as a Git repository.
13. Committed the laboratory files.
14. Pushed the repository to GitHub.

## Linux Commands Used

```bash
whoami
pwd
hostname
ls
adduser kpadilla
usermod -aG sudo kpadilla
groups kpadilla
getent passwd kpadilla
su - kpadilla
cat /etc/os-release
uname -r
lscpu
free -h
df -h
cd
mkdir
touch
mv
cat
nano
tree
git init
git status
git add
git commit
git remote
git push


## Skills Learned

Through this activity, I learned how to access and work inside a cloud-based Linux environment. I practiced using basic Linux commands to navigate directories, inspect system information, create users, and organize files.

I also learned that documentation is an important part of technical work. Instead of only completing commands, I had to record what I did and provide screenshots as evidence.

Another important skill I practiced was using Git and GitHub. I learned how a local project can be tracked using Git and then uploaded to a GitHub repository. This will be useful for keeping my future laboratory activities organized in one portfolio.

Overall, this activity helped me become more comfortable with the Linux terminal and gave me a better understanding of how cloud engineers organize and document their work.
