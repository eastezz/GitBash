# Pull Request Tutorial

## What is a Pull Request?

A Pull Request (PR) is a request to merge your branch into another branch (usually `main`).

It is commonly used on GitHub for code review and collaboration.


## When to Create a Pull Request

After pushing a feature branch:

```bash id="zkm2rb"
git push origin feature-name
```

GitHub will show a button:

👉 "Compare & pull request"


## Pull Request Workflow

1. Create a branch
2. Make changes
3. Commit changes
4. Push branch
5. Open Pull Request
6. Review and merge


## Why Pull Requests Are Important

PRs allow teams to:

* review code
* discuss improvements
* detect bugs early
* maintain quality


## After Merge

Once merged:

* your changes become part of the main project
* the branch can usually be deleted


## Professional Tips

* Keep PRs small and focused
* Write clear descriptions
* Link related issues
* Respond to review comments


## Example Feature Development

```bash id="9ubgza"
git checkout -b login-feature
# develop feature
git add .
git commit -m "Implement login system"
git push origin login-feature
```

Then open a Pull Request on GitHub.


## Why Recruiters Care

Understanding pull requests shows you can:

* work in teams
* follow professional workflows
* contribute to real projects
