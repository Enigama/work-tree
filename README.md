# work-tree
We have 3 ways how we can clone the project:
1) simple git clone without flags
2) bare clone -> git clone --bare -> This approach doesn't allow us to get remote updates fully, so basicly we can use git pull, push even fetch but we'll get updates only for branches which was created when we cloned the project or for branches which we created in bare repo locally and pushed it to remote.
3) mirror clone -> git clone --mirror -> Here we can have full powe of git pull, fetch ant etc. the main instruction if we want to have update branches we shuld create them out of mirror repo here where comes worktree flow

Reccomendation when and which approach can be usefful:
1) If you work on the project that doesn't make you to work on some fixes/feature while you are working on another feature/fix in short you don't need to swicht branches quiet frequently.
2) Clone with --bare flag could be used for many approaches: 
    1) For storing your dotfiles, as we know system configs(dotfiles) could be stored in different folders here when we can use bare repo and setup our git config to add once all our files to traking and        forget about it, and if we need to update our files from git than we could easy to pull date without any extra steps like sym linking.
    
