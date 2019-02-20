# How to delete a file with a path 'too long to be deleted'

We will use [subst](https://ss64.com/nt/subst.html) command.

- Start a command prompt `cmd` and navigate to the destinate folder, or type `cmd` to the address bar in it.
- Run `subst j: .` to create the driveletter association.
- Now in Explorer you have a new drive letter in *This PC*. Go to it and do whatever you need to do (delete, rename or whatever).
- Return to your cmd window and type `subst /d j:` to remove the drive or alternatively restart your PC.
