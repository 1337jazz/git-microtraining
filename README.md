
### Objective
The objective of this training is to:

- make you more comfortable with the `terminal` git commands, instead of being reliant on GUIs
- teach you some tips and tricks with git to make your day-to-day workflow more streamlined
- Get a little deeper into git to really understand what's going on under the hood with common  issues you might 

***
## Working with Branches
---
### Creating branches

- Create a branch:
>`git branch <branch-name>`

- Checkout a branch
>`git checkout <branch-name>`

- Create a new branch and switch to it:
>`git checkout -b <branch-name>`
>
**or**
>
>`git switch -c <branch-name>`

**Recommendation**: use `git switch` for simple tasks around switching and creating branches. `git checkout` has many more function.


###  Deleting branches

- Switch to any other branch
> `git switch <other-branch>`

- Now you can delete the branch
> `git branch -d <branch-to-delete>`


#### Force delete
If the branch you want to delete has uncommited changes, you might get this message:
```
The branch <branch-to-delete> is not fully merged
```

To force the delete, simply use a capital "D" for the delete flag in the previous command:
>`git branch -D <branch-to-delete`



### Renaming branches

- Switch to the branch you want to rename - **note**: unlike the delete command, with which you need to be on **any other branch**, you must be on the branch you want to rename
>`git branch -m <old-name> <new-name>` <-- "-m" stands for "move"

