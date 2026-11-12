
# Lab 4 — Git & GitHub Notes

## Question 1
`--global` means the Git configuration is applied to the current user's Git configuration across all repositories on the computer. If `--global` is omitted, the setting applies only to the current repository.

## Question 2
`ls -a` shows hidden files and directories as well as normal files. The important new item is `.git`, which contains Git's repository metadata, including the object database, references, configuration, and index.

## Question 3
The exact number depends on the contents of my `coding-cafe` folder. Before creating `.gitignore`, `git status` may list many files, especially files inside `.venv/`. The files I did not write myself are mainly virtual-environment and generated/cache files.

## Question 4
After creating `.gitignore`, files inside `.venv/`, `__pycache__/`, `*.pyc`, and `.DS_Store` no longer appear as untracked files. The `.gitignore` file itself appears as an untracked file because Git tracks the ignore-rules file itself.

## Question 5
`.gitignore` should be committed because it is part of the project's configuration and tells future users which files should not be tracked. It should not be ignored because the repository needs to preserve its own ignore rules.

## Question 6
`README.md` moves from the untracked/unstaged area to the staged changes area after `git add README.md`. In the three-places model, its changes have moved from the working tree to the staging area (index), ready for the next commit.

## Question 7
After `git commit`, Git prints information about the new commit, including the commit ID, branch, commit message, and a summary of files changed, insertions, and deletions. The exact number of changed files depends on the contents of my `coding-cafe` folder when I ran `git add .`.

## Question 8
The first seven characters are the abbreviated commit hash (commit ID). They identify a particular commit in the repository's history.

## Question 9
The four steps are:
1. Edit or create files.
2. Stage the changes with `git add`.
3. Commit the staged changes with `git commit`.
4. Repeat the cycle when further changes are made.

## Question 10
`README.md` is special because GitHub automatically renders it on the repository's front page. It is placed in the repository root so visitors immediately see the project's description, instructions, and contents.

## Question 11
`gh auth login` authenticates the GitHub CLI with my GitHub account and stores the authentication credentials/token securely. This allows Git operations through the configured GitHub authentication without repeatedly entering a GitHub password.

## Question 12
The GitHub repository's front page shows `README.md` as formatted text. GitHub automatically renders the root `README.md` on the repository's main page.

## Question 13
No. `git push` does not change the local commit history. It copies commits that already exist locally to the remote repository on GitHub.

## Question 14
A private repository exists on GitHub but its contents can only be accessed by the owner and people who have been granted permission. If a repository does not exist on GitHub at all, there is no remote GitHub repository to access, collaborate on, or push to.

