# Remove .DS_Store Files from git Repositories

In this article, I am explaining how to remove .DS_Store files from your git repositories.

## What is .DS_Store file

.DS_Store stands for Desktop Services Store and it holds meta-information about your folder’s thumbnails, settings, etc. in macOS operating system.

.DS_Store files are created any time you navigate to a file or folder from the Finder on a Mac.

## How to remove .DS_Store files?

### Remove .DS_Store files from current directory?

If you have .DS_Store files in your folder, then copy and paste this commands to remove the file from current directory:

git rm --cached .DS_Store

git add .

git commit -m "Remove .DS_Store from current directory"

git push origin master

### Remove .DS_Store files from all over project?

If you have .DS_Store files all over your project, then copy and paste this commands to find and remove all of the files from the repository:

find . -name .DS_Store -print0 | xargs -0 git gm --ignore-unmatch

git add .

git commit -m "Remove .DS_Store from everywhere"

git push origin master

## How to always ignore .DS_Store files?

Let’s make a global .gitignore file:

echo .DS_Store >> ~/.gitignore_global

And let git know that you want to use this file for all of your repositories:

git config --global core.excludesfile ~/.gitignore_global
