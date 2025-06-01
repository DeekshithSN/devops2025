📘 README: Git Commands for Beginners - DevOps Training

This guide covers the basic Git commands explained during our AWS & DevOps training. It's written in a step-by-step flow to help beginners work with Git confidently from start to finish.

👤 Author: Sai Manikanta
📅 Created during: AWS & DevOps Training
📁 File Type: README.txt

------------------------------------------------------------
🔧 1. SETUP PHASE (Before you start)
------------------------------------------------------------

👉 Make sure Git is installed on your system. You can verify by:
   $ git --version

👉 Configure Git with your name and email:
   $ git config --global user.name "Your Name"
   $ git config --global user.email "you@example.com"

------------------------------------------------------------
📥 2. CLONE A REMOTE REPOSITORY
------------------------------------------------------------

📌 Command:
   $ git clone https://github.com/username/repository.git

📖 Use this when you're starting work on an existing project.
💡 It copies all files and Git history to your local machine.

------------------------------------------------------------
🌱 3. WORKING WITH BRANCHES
------------------------------------------------------------

🔹 Create a new branch:
   $ git branch feature-branch

🔹 List all branches:
   $ git branch

🔹 Switch to a branch:
   $ git checkout feature-branch

🔹 Create & switch in one step:
   $ git checkout -b new-feature

------------------------------------------------------------
🌍 4. REMOTE REPOSITORY SETUP
------------------------------------------------------------

🔹 Add a remote repo (if not cloned):
   $ git remote add origin https://github.com/user/repo.git

🔹 View connected remotes:
   $ git remote -v

------------------------------------------------------------
📦 5. STAGE FILES FOR COMMIT
------------------------------------------------------------

🔹 Add a specific file:
   $ git add filename.txt

🔹 Add all modified files:
   $ git add .

📌 This prepares files to be saved in Git history.

------------------------------------------------------------
📝 6. COMMIT CHANGES
------------------------------------------------------------

🔹 Commit staged changes:
   $ git commit -m "Added login feature"

💡 Commits are saved snapshots of your work.

------------------------------------------------------------
🚀 7. PUSH CHANGES TO REMOTE (using SSH)
------------------------------------------------------------

🔹 Set SSH URL (if not set already):
   $ git remote set-url origin git@github.com:user/repo.git

🔹 Push your code to main branch:
   $ git push origin main

✅ Make sure your SSH key is added to GitHub before this.

------------------------------------------------------------
🔍 8. CHECK STATUS OF YOUR WORK
------------------------------------------------------------

🔹 See current Git status:
   $ git status

📌 Shows what's modified, staged, or untracked.

------------------------------------------------------------
📜 9. VIEW COMMIT HISTORY
------------------------------------------------------------

🔹 Full history:
   $ git log

🔹 Short version:
   $ git log --oneline

👀 Useful to track who did what and when.

------------------------------------------------------------
🔀 10. MERGE CHANGES FROM ANOTHER BRANCH
------------------------------------------------------------

🔹 Merge feature branch into main:
   $ git checkout main
   $ git merge feature-branch

💡 Brings the work from one branch into another.

------------------------------------------------------------
🔄 11. PULL CHANGES FROM REMOTE
------------------------------------------------------------

🔹 Fetch and merge in one step:
   $ git pull origin main

📌 Keeps your branch updated with latest remote changes.

------------------------------------------------------------
📥 12. FETCH WITHOUT MERGING
------------------------------------------------------------

🔹 Download changes from remote:
   $ git fetch origin

📌 Downloads updates but does NOT merge them automatically.

------------------------------------------------------------
🛠️ 13. AMEND THE LAST COMMIT
------------------------------------------------------------

🔹 Change last commit message or add forgotten file:
   $ git commit --amend -m "Updated commit message"

🔹 If force-push is needed after amend:
   $ git push origin branch-name --force

⚠️ Only use this if the commit is NOT yet pushed or if you're sure.
📌 It rewrites commit history.

------------------------------------------------------------
💡 PRO TIPS FOR USING GIT
------------------------------------------------------------

✅ Use `git status` often to avoid mistakes
✅ Always work on a separate branch when building new features
✅ Use meaningful commit messages (what and why)
✅ Prefer SSH over HTTPS for pushing (secure + easy)
✅ Before pushing, always pull the latest changes to avoid conflicts

------------------------------------------------------------
📣 Final Note

This is your core Git workflow. Master these steps before moving to advanced concepts like rebase, stash, cherry-pick, etc.


