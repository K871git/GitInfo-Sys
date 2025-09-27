*name changed from Infosys to the Git all in one repo
modifying this git repository again

* ISSUE OF THE the mighty (END) — guardian of long outputs in VS Code's terminal. You're bumping into a built-in pager called less, which Git uses to help scroll through long results like git log or git diff.

# 💡 Why You’re Seeing (END)
When the output is too long for one screen, Git pipes it through less, a terminal program that:
  Lets you scroll one page at a time.
  Shows (END) when you're at the bottom.
  Blocks normal typing unless you give it specific keys.

# 🔓 How to Exit the Pager
When stuck at (END):
  Press q — it quits the pager and returns you to your terminal.
  Use ↑ or ↓ to scroll line-by-line.
  Use Space to page down.
  Use b to page up.


# BRANCH MATRICS :
    # git branch :- check current branch 
    # git branch -r
    # git branch -a : showing all the local branches ( the branch with * is the HEAD pointer's home)
    # git remote show origin : show Default HEAD branch and remote branch stuff 

    # git checkout <branch name> : 
      git checkout -b newLocal :  this command create new local branch and switch to them : so localy newLocal is present where remote not
      git push -b newLocal : this command will push the local branch to the remote and set it for track future pull and push

    # If the branch doesn’t exist locally, you’ll get an error like:
        fatal: 'main' cannot be resolved to branch
    
# 🧯 Fix: "fatal: main cannot be resolved to branch"
        # checkout remote branches : if the output looking like this : origin/main then : then add it for tracking local changes
            git checkout -b main origin/main :like this I can add any branch to the local for tracking

        and if you dont know the default branch name then just type : git remote show origin 
        this command will show about default branch name : HEAD master : then switch to the master using command :
        git checkout master
        and 
