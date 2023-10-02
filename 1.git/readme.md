## 1. Git
Git allows us to version control our code, helping us manage our code merges.

Typically we would have a single branch (commonly called `main`, previously `master`) that acts as the production ready codebase. We can then create branches (or copies of this `main` branch) from which we can make our code changes without affecting the production codebase. Once our code changes are ready we can merge them into `main`, git will figure out what's new and only merge these into the main branch without affecting the rest of the codebase. The most common commands are:

 - `git status` - this will show us the current branch we are on and the state that it's in, e.g. it should show any modified files

 - `git fetch` - this will fetch any new branches in the remote repo in github onto our laptops, e.g. if someone else has pushed up a new branch, we can see this locally by running `git fetch`

 - `git clone` - this function will pull down a repo onto your local machine, an example would be `git clone https:`

  - `git checkout -b feature-branch` - this will create a copy of the current branch called `feature-branch`, e.g. if we are on the `main` branch and run `git checkout -b feature-branch`, this would create a copy of the `main` branch on `feature-branch`

  - `git checkout` - this allows us to move between branches, e.g. `git checkout main` or `git checkout feature-branch`

  - `git add` - once code changes have been made to a file we can 'stage' these changes so that they are ready to be pushed up into github, e.g `git add index.html`

  - `git commit` - when code changes have been staged, this will create a snapshot of the branch that is ready to be pushed up to github, e.g. `git commit -m "Updated homepage text"`

  - `git push` - once changes have been staged and commited we can push these up into github this will 'save' our work in github, e.g. `git push origin feature-branch`

  - `git pull` - this will download any code changes that have been made to a branch, e.g. if someone has pushed up code changes to a branch we're working on, we can run `git pull` to download these onto our laptops

  - `git merge` - this will attempt to merge one branches code changes into another, e.g. `git merge origin main`


## Using git
First task is going to be pulling down a repo, creating a branch, making an amend to a file and then merging that into the main branch.

 1. `Clone` this repo onto your laptop
 1. create, or `checkout`, a new branch so that we can make changes without changing the code in the `main` branch
 1. open `index.html` in any text editor, and change the text from `Hello World!` to anything you want
 1. Once you've done this, stage, or `add` these changes
 1. `commit` these changes so we create a snapshot of the branch
 1. Then `push` the changes made to this new branch up to github
