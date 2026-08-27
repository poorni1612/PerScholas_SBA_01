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