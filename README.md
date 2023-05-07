# work-tree
We have 3 ways how we can clone the project:
1) simple git clone without flags
2) bare clone -> git clone --bare -> This approach doesn't allow us to get remote updates fully, so basicly we can use git pull, push even fetch but we'll get updates only for branches which was created when we cloned the project or for branches which we created in bare repo locally and pushed it to remote.
3) mirror clone -> git clone --mirror -> Here we can have full powe of git pull, fetch ant etc. the main instruction if we want to have update branches we shuld create them out of mirror repo here where comes worktree flow
