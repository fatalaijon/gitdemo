## Summary of Git commands:

* git init - create a new repository
* git status - compare working directory with local repository
* git add file1 file2 ...  - mark files for adding or update in local repository
* git commit -m "write a good commit message" - save staged files to repository
* git lost

## Connecting to Github

### Case 1:  Copy a local project to Github

If you already have a local project and a local git repository containing project files.

1. Create a new **empty** repository on Github
2. Give it a name. Use the name the instructor specifies for assignments.
3. Copy the URL that Github shows you.
4. Inside your local project, add github as remote:
```shell
cmd> git remote add origin https://github.com/fatalaijon/gitdemo.git
```
5. Push (copy) the local repo to Github:
```shell
cmd> git push -u origin master
```

### Case 2: Copy (clone) a Github project to your computer

If the project already exists on Github then do:

1. In web browser, go to the project page on github so you can get the URL
2. Click the "Clone or Download" button. This will show the URL of the project. It also gives instructions.
    * There is a button to copy this URL directly to your clipboard
3. In the **parent directory** of where you want to clone the project, enter:
    ```shell
    cmd> git clone https://github.com/fatalaijon/someproject.git
    ```
    This creates a local directory having the same name as remote repository ("someproject" in this example).
4. If you want to use a different name for your copy of the remote (Github) repository, then type:
    ```shell
    cmd> git clone  https://github.com/fatalaijon/someproject.git  myproject
    ```
    in this case, git will create a directory named `myproject` and copy the project there.

When you clone a project, git remembers the "upstream" location. So you can push (upload) you
local changes to  the project using `git push`.

Jim Brucker
