# ACP

ACP stands for:

- Add 
- Commit
- Push

One thing I learned here is that one should not run the **git add filename** command until after changes have been made. Otherwise git does not reflect the changes.

## Process

Here is the process.

1. Using terminal, navigate to location where you want to clone repository.

2. In GitHub, get clone link.

3. In terminal, type **git clone *address*** (copied clone address from GitHub)

4. CD to cloned repository.

5. Use **code .** to open VSCode.

6. Make edits locally in VSCode.

7. In terminal, **git add**

8. In terminal, **git status**. This will show changes that need to be committed, pushed.

9. In terminal, **git commit -m "*note*** (note should be what and why changed).

10. In terminal, **git push origin main**