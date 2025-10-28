🧠 GIT COMMANDS — COMPLETE CHEATSHEET
⚙️ 1️⃣ Setup Git (first time only)
git config --global user.name "your username"
git config --global user.email "your email"

📦 2️⃣ Initialize a Repository
git init

📥 3️⃣ Add Files
git add filename.ext     # Add a single file
git add .                # Add all files

💾 4️⃣ Commit Changes
git commit -m "Your commit message"

🌐 5️⃣ Connect Local Repo to GitHub
git remote add origin https://github.com/"your username"/repo-name.git

🚀 6️⃣ Push to GitHub
git branch -M main
git push -u origin main

🔁 7️⃣ Pull Updates from GitHub
git pull origin main

🌿 8️⃣ Branch Commands
git branch                 # List branches
git branch new-branch      # Create new branch
git checkout new-branch    # Switch to branch
git checkout -b new-branch # Create & switch
git merge new-branch       # Merge branch into current
git branch -d branch-name  # Delete branch (safe)
git branch -D branch-name  # Delete branch (force)
git push origin --delete branch-name  # Delete remote branch

🔄 9️⃣ Undo / Reset / Revert
git reset HEAD filename          # Unstage file
git reset --soft HEAD~1          # Undo commit, keep changes
git reset --hard HEAD~1          # Undo commit, remove changes
git revert <commit-id>           # Revert specific commit
git checkout -- filename         # Restore a file to last commit

🗑️ 🔟 Delete / Force Commands
git rm filename                  # Delete file from repo
git rm -rf filename              # Delete file/folder (force)
git add -f filename              # Force add ignored file
git push origin main --force     # Force push (overwrite remote)


⚠️ Warning: --force replaces code on GitHub with your local version!

🧭 1️⃣1️⃣ Status & Logs
git status                       # Show current status
git log                          # Full commit history
git log --oneline                # Short history
git diff                         # Show code differences
git remote -v                    # View remote URLs
git config --list                # View all config settings

🔧 1️⃣2️⃣ Manage Remote
git remote remove origin
git remote add origin https://github.com/nzm-777/repo-name.git

🧹 1️⃣3️⃣ Clean Workspace
git clean -f                     # Remove untracked files
git clean -fd                    # Remove untracked files/folders

📦 1️⃣4️⃣ Clone Repository
git clone https://github.com/nzm-777/repo-name.git

💪 1️⃣5️⃣ Stash Commands
git stash                        # Save uncommitted changes
git stash list                   # List stashes
git stash apply                  # Apply last stash
git stash drop                   # Delete last stash

🧍‍♂️ 1️⃣6️⃣ Compare Branches
git diff main new-branch

🔒 1️⃣7️⃣ Tag Versions
git tag v1.0
git push origin v1.0

💣 1️⃣8️⃣ Remove Git Tracking
rm -rf .git

⚡ Bonus: Full Workflow to Upload a Project
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/"your username"/repo-name.git
git push -u origin main

