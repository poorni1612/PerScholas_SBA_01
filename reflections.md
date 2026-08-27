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