# How to add locally hosted code to GitHub
Mon. Feb. 10, 2025

Follow the steps on this page to add locally hosted code to GitHub:
https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github

Some notes:
* To push to a private remote repo, you may need to enter your user name and password. For your password you actually need to enter your fined-grained access token from GitHub, not your password to your GitHub account.
    * It's a bit slow copying in your fine-grained acces token each time, but I haven't found if there's a way to not have to enter it each time
* To commit changes to a file that is being tracked, use the same command for adding an untracked file: `git add my_file.txt`.
* To add all files in a directory, use the star: `git add my_dir/*`
