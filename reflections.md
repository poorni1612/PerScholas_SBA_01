Steps to create Repo,Branches, Push, Merge,Pull
Create a repo on GitHub Go to GitHub → New Repository → give it a name → Create.

Create a new branch
   git checkout -b feature/my-feature
Make your changes Edit/add files in your project as needed.
Stage the changes
   git add .
Commit the changes
   git commit -m "Describe what you changed"
Push the branch to GitHub
   git push -u origin feature/my-feature
Create a Pull Request
   gh pr create --fill
(or open the branch on GitHub.com and click "Compare & pull request")
Merge the Pull Request
   gh pr merge --merge
(or click "Merge pull request" on GitHub.com)
Pull the latest changes into your local main
    git checkout main
    git pull
Here's the simplest day-to-day version, all from the VS Code terminal (Terminal menu → New Terminal, or Ctrl+`):

Create (first time, brand new project)

git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/yourusername/repo-name.git
git push -u origin main

Or, if the repo already exists on GitHub — just clone it:

git clone https://github.com/yourusername/repo-name.git

Push (after editing files)

git add .
git commit -m "Describe what you changed"
git push

(after the first -u push, plain git push works from then on)

Pull (get the latest changes down)

git pull
