## Making changes to the codebase in your branch

Now that you know how to create a branch to make your changes, time to actually make the changes!

Doing so is pretty self-explanatory, once you're in your branch, edit files however you see fit. You can add and delete files, reorganize directories, and change code and Git will track it all. 

Once you're ready to actually push these changes, they need to be staged and then bundled in a commit. Think of staging as telling Git "Hey, these are the files I'd like to group together." and then making a commit is actually doing the bundling.

Commits are how Git tracks different changes to the codebase. Normally, we'd like to make commits as small as possible so that we have a record of how the repository is changing. Better to have a lot of small commits rather than a few big commits. Also, if something goes wrong in the code we can always revert the repo to a prior commit. 

#### To stage a file for commit, enter: 
```
git add <file_path>
```
#### to stage all altered files, enter:
```
git add .
```
**Note:** It is much more common to just stage every altered file rather than pick and choose. However, if you only want to bundle certain files in a commit then feel free to do so.

#### To bundle a commit, enter:
```
git commit -m <commit_message>
```
Where `<commit_message>` is a message describing what your commit does. To use the Pong example from before, a good description would be something like `"allows user to change the background color"`.

#### To check the status of your files, enter:
```
git status
```
This is a very helpful command in showing you which files are and aren't staged. It also provides helpful commands to undo staging and commits if you ever need to do so.

## Challenge 3:

1. Create a file in the `people` subdirectory with your first and last name titled `firstname_lastname.txt`. 
2. Put a random sentence inside. 
3. Add a line containing your name to the comment in `printer.py`
4. Run `python run.py` to see your name added to the chain! Change your own file as much as you'd like.
5. Stage the files and bundle them in a commit.

[Next: Push your local changes to GitHub](../part5-pushing_changes_to_github)

Code Changed for Testing purposes