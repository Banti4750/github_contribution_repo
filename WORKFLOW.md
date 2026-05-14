# Contribution Workflow

A repeatable checklist for contributing to an open source project.

## 1. Pick a repo / issue
- [ ] Read the README and `CONTRIBUTING.md`
- [ ] Check the project is active (recent commits, maintainers respond to PRs)
- [ ] Look for issues labeled `good first issue`, `help wanted`, `up for grabs`
- [ ] Comment on the issue to ask if you can take it

## 2. Set up
- [ ] Fork the repo, then clone your fork
- [ ] Add upstream: `git remote add upstream <original-repo-url>`
- [ ] Install deps and run the build/tests to confirm a clean baseline
- [ ] Create a branch: `git checkout -b fix/short-description`

## 3. Make the change
- [ ] Keep the change small and focused on the issue
- [ ] Follow the project's code style and conventions
- [ ] Add or update tests
- [ ] Run the full test suite + linter

## 4. Submit
- [ ] `git commit` with a clear message (follow their commit style)
- [ ] Push to your fork, open the PR against upstream
- [ ] Reference the issue (`Closes #123`) and describe what + why
- [ ] Fill out their PR template fully

## 5. Follow up
- [ ] Respond to review comments promptly
- [ ] Keep your branch up to date: `git fetch upstream && git rebase upstream/main`
- [ ] Once merged, log it in [CONTRIBUTIONS.md](CONTRIBUTIONS.md)

## Staying in sync (your fork)
```
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```
