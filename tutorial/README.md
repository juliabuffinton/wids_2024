# Tutorial 
## Set Up

1. Open up Git Bash (Windows) or terminal (Mac/Linux). Type the following commands (press enter between each) to set your name and email. Change "Your Name" and "Your Email" to your actual name and email, or whatever you would like displayed alongside your commits.

`git config --global user.name "Your Name"`

`git config --global user.email "Your Email"`

## Create a Repo
There are multiple ways you might initiate a local git repository:
1. Create a new repository locally (that you might ultimately track remotely).
2. Create a new repository on the remote server (e.g., Github).
3. Clone an existing repostory on Github, either yours or someone else's.

We're actually going to do this the second way, because then we can also get familiar with Github, and it is (in my opinion) a little easier to set up.

1. Go to [Github.com](https://github.com) and create a new repository by clicking the green "New" button on the left side.
2. Give your new repo a fun name! Git will suggest one; take its suggestion by clicking on the green text after "How about...?"
3. Make sure your repo is public and check "Add a README file" under the Initialize header. Create your repository.

Tada!

## Configure Repo
Every repo is different, and there are many ways to configure each to meet their specific need. 

1. Go to "Settings" along the top menu bar.
2. On the first page ("General") make sure your default branch is set to `main`. If not, change it!
3. Under "Code and automation" click on "Branches". Practice adding a branch protection rule where the "main" branch requires a pull request before merging. **Do not save!** This is a best practice for individual and collaborative code development; it's a handy guardrail preventing accidental pushes of code to the production branch. For more about branch protection, visit [this link](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rulegit).

## Clone Your Repo

1. In Git Bash or terminal, navigate to the directory you'd like to put this repo in (e.g., the directory that will be the parent of your repo). **It is very important that you do NOT clone this repository into an existing git-tracked repository.**

   Option A: using file explorer, navigate to the directory. Copy the address. In Git Bash, type `cd ` (note the space after cd) and then paste the address (SHIFT+INS).
   Option B: within Git Bash, navigate to your directory using `cd ` command.

2. In Github, go back to "Code" in the top menu bar.
3. Click the green "<> Code" button in the upper right. Make sure you are on the **HTTPS** tab; copy the URL to your clipboard.
4. In Git Bash, type `git clone ` (note the space after clone) and then paste (SHIFT+INS) the URL. 
5. Navgiate into to that repository by typing `cd <your_repo_name>`.

Branch protection:
You can create a branch protection rule in a repository for a specific branch, all branches, or any branch that matches a name pattern you specify with fnmatch syntax. For example, to protect any branches containing the word release, you can create a branch rule for *release*.


https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rulegit 
