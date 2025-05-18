# 08-open-vscode-in-folder.md

Now, we use our new tools to verify our setup.
Be sure you have completed all earlier steps successfully and you have a `Repos` folder that is not automatically synced.

## VS Code Editor is Folder-based / Project-based 

VS Code is a **folder-based editor**. 
That means everything we do—whether editing files, running code, or using Git assumes that we’ve opened a specific folder.
If we open VS Code without opening a folder, many features may not work as expected. For example:

- The terminal might not open
- Python environments might not be detected
- Git integration may fail to activate

**Always start by opening a folder in VS Code.** 
In this course, that will usually be a project folder inside the `Repos` folder.
We may not have any GitHub project repos yet, so we'll work in the `Repos` folder for now. 

---

## Open VS Code in Your Repos Folder

### Option 1 (Graphical):

1. Open your `Repos` folder using File Explorer (Windows) or Finder (Mac).
2. Right-click on the folder and choose **"Open with Code"**.

### Option 2 (Terminal, if configured):

If you installed the `code` command in your terminal (e.g., using the Command Palette), you can type one of the following, the first works in Mac or Linux, the second command works in Windows PowerShell:

- `code ~/Repos`
- `code C:\Repos`

Either option should open your Repos folder in VS Code.

---

## Using the Integrated Terminal in VS Code

Once you’ve opened a folder in VS Code:

1. Go to the top menu and select **Terminal** > **New Terminal**.
2. A terminal will appear in the lower part of the VS Code window.

This is called the **integrated terminal**. You can run commands here just like in your regular system terminal.

### Terminal Types

On most systems, VS Code defaults to the system’s default shell:

- **Mac or Linux**: zsh or bash
- **Windows**: PowerShell, Command Prompt, or Git Bash (if installed)

You can change your default shell by clicking the dropdown next to the plus sign (`+`) in the terminal tab.

---

## Troubleshooting: Terminal Won’t Open in VS Code (Windows)

Some Windows users find the terminal in VS Code won’t open if no folder is loaded. This is a known issue, especially if:

- You opened VS Code without a folder
- You’re using a secondary drive (like D:\)
- No default working directory is configured

### Solution

1. In VS Code, go to **File > Preferences > Settings**
2. In the search box, type: `terminal.integrated.cwd`
3. Set this field to a valid folder path like `C:\Repos`

This ensures that the terminal has a default folder to open in—even when VS Code is opened without a project.

---

## Professional Practice: Always Open a Folder First

Whenever you start working, make sure you open the correct project folder inside your `Repos` directory. This ensures that:

- The terminal opens correctly
- Git works properly
- Python environments are detected
- VS Code features behave as expected

---

## Verify Installations

On Mac/Linux:

```shell
python3 --version
pip3 --version
git config --list
```

In Windows PowerShell:

```powershell
py --version
pip --version
git config --list
```

Make sure your version commands show numbers and your config lists your user.name and user.email.
If not, return to the instructions and redo the tasks until success. 
You need these tools installed and configured to complete the projects. 

---

[🟢 Back to Part 1 Home](https://denisecase.github.io/pro-analytics-01/01-machine-setup/MACHINE-SETUP.html) | [🔗 View Part 1 on GitHub](https://github.com/denisecase/pro-analytics-01/01-machine-setup/MACHINE-SETUP.md)
