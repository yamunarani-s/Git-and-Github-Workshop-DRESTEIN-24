# Git-and-Github-Workshop-DRESTEIN-24
NAME:  YAMUNA RANI S
REGISTER NUMBER :  212223060309
DEPARTMENT :  ECE
YEAR :  SECOND YEAR
1. Setup and Initialize: - What command do you use to create a new directory named `git-workshop and navigate into it?

mkdir git-workshop   # Creates a new directory called 'git-workshop'
cd git-workshop      # Changes the current directory to 'git-workshop'

2. Initialize a Git Repository: - What command initializes a Git repository in your directory?

git init
3. Create and Modify Files: - How do you create a new file named `hello.txt` and add the content 'Hello, Git
echo "Hello, Git" > hello.txt

git status
. 4. Check the Status of Your Repository: - What command displays the status of your repository?
git status

This command shows information about the current state of the repository, including any files that are staged, unstaged, or untracked.
5. Stage and Commit Changes: - What command stages the file `hello.txt`? - What command commits the staged file with the message 'Add hello.txt with welcome message'?
To stage the file hello.txt, use the following command:
git add hello.txt
To commit the staged file with the message "Add hello.txt with welcome message", use the following command:
git commit -m "Add hello.txt with welcome message"


6. Branching: - What command creates a new branch named `update-content`? - How do you switch to the `update-content` branch?

To create a new branch named update-content, use the following command:
git branch update-content

To switch to the update-content branch, use:
git checkout update-content

Alternatively, you can create and switch to the new branch in a single command:
git checkout -b update-content


7. Make Changes on the Branch: - What command would you use to append the text 'This is a simple Git assignment.' to `hello.txt`? - What command stages and commits the changes with the message 'Update hello.txt with additional message'?

To append the text "This is a simple Git assignment." to hello.txt, use the following command:
echo "This is a simple Git assignment." >> hello.txt

To stage and commit the changes with the message "Update hello.txt with additional message," use:
git add hello.txt
git commit -m "Update hello.txt with additional message"

8. Merge Changes: - What command switches you back to the `main` branch? - How do you merge the `update-content` branch into `main`?
To switch back to the main branch, use the following command:

git checkout main

To merge the update-content branch into main, use:
git merge update-content

This command combines the changes from update-content into main.

9. View Commit History: - What command shows the commit history?

git log

This command displays a list of commits in the repository, including details such as commit IDs, author names, dates, and commit messages. For a more compact view, you can use:
git log --oneline
This option shows each commit on a single line with its ID and message.


10. Undo and Reset (Practice Safely): - If you make a change to `hello.txt` that you want to revert before committing, what command would you use? - How can you reset your branch to a previous commit (optional, for advanced practice)?

If you make a change to hello.txt that you want to revert before committing, you can use the following command to discard the changes:
git checkout -- hello.txt

This command resets hello.txt to the last committed state, effectively undoing any uncommitted changes.
For resetting your branch to a previous commit (optional for advanced practice), you can use the git reset command. For example, if you want to reset to a specific commit (let's say the commit ID is abc123), you can use:
git reset --hard abc123

This command will reset your branch to the specified commit, discarding all changes made after that commit. Be cautious when using --hard as it will permanently delete any uncommitted changes. If you want to keep your changes in the working directory, you can use:

git reset --soft abc123

This will keep your changes staged for commit.
11. Push to a Remote Repository (Optional): - What command adds a remote repository named `origin`? - What command pushes your local `main` branch to the remote repository?
To add a remote repository named origin, you can use the following command, replacing URL with the actual URL of your remote repository:
git remote add origin URL

To push your local main branch to the remote repository, use:

git push origin main

This command uploads your local main branch to the remote repository named origin.

