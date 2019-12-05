# GitHub Tutorial

_by Dennis Grigoryev_

---
## Git vs. GitHub
Git: Programming language that allows the developer to keep snapshots of code and back-track to previous codes
GitHub: Place where coding is stored, specifically git. Github also tracks the changes made to files and/or repositiories.

---
## Initial Setup
**config** - Used to shape/order/put together or order something
### To Start using git and GitHub, follow the steps below!
1. Use git config --global user.email "you@example.com"
    - Example: git config --global user.email "_dennisg8153@hstat.org_"
2. Then type git config --global user.name "Your Name"
    - Example: git config --global user.name "_DennisG8153_"
3. Do cd ~ (makes sure you are in the root directory)
4. Type in ssh-keygen -t rsa -b 4096 -C "you@example.com" (**Make sure you keep pressing Enter slowly until you see a werid block of text.)
    - Example: ssh-keygen -t rsa -b 4096 -C "_dennisg8153@hstat.org_"
    - Your screen should post this: The key's randomart image is:

+--[ RSA 4096]----+
|       .o o..    |
|       o +Eo     |
|        + .      |
|         . + o   |
|        S o = * o|
|           . o @.|
|            . = o|
|           . o   |
|            o.   |
+-----------------+ (**Remember, it's different every time!**)
5. Do ls -al ~/.ssh (List all files long and looks for ~/.ssh), you should now see a file named *id_rsa.pub*
6. Do cat ~/.ssh/id_rsa.pub (Opens the thing to a **LOT** of text)
7. Copy the entire result to your clipboard (it should start with ssh-rsa and end with your email address)
8. Go to (https://github.com/settings/keys) --> New SSH Key
9. Title the key: ide50
    - Key: paste your ssh key
10. Press the green Add SSH key button
11. Go back to your cs50 IDE
12. Do sudo nano ~/.ssh/config
13. When inside the window: paste the following block of text.
Host github.com
 Hostname ssh.github.com
 Port 443
14. Press _Control X_ to exit, then _press the Y key_ then the _ENTER key_
15. Type: ssh -T git@github.com
16: Type yes, press ENTER, and you should see
> Hi "username"! You've successfully authenticated, but GitHub does not provide shell access.
    - Example: Hi "DennisG8153"! You've successfully authenticated, but GitHub does not provide shell access.

---
## Repository Setup



---
## Workflow & Commands
