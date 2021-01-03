# git-fix
Fixes your .git by murdering it and replacing it with a clean one. Use at your own risk!

All local .git changes will be lost. This is not recommended for serious use, but I find myself using it a lot for personnal projects. I am not responsible for any loss of data/code/etc. resulting from using this script.

# What it does

This clones your original repo, rips out the .git file, and replaces your original one with it. Any unpushed .git changes will be lost, even if they were committed (but your local files will stay the same!). For example, this is useful when you mess up and commit a file which requires git LFS, which is very annoying to fix.

Instead of messing with your .git, you can `git fix` and replace your .git with a clean one from your repo's source.

This takes branches into account.

# Usage

Simply type `git fix` as though this script was an actual git command. 

# Install

Run `install.sh`. This will add `git-fix` to your `/home/$USER/.local/bin`.
