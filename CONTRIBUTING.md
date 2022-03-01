# FRONTEND

## HOW TO CONTRIBUTE

You can download the project and run it locally based on the description that is usually placed at README.md.

Make any required changes there and commit your changes. You can find how we commit [here](https://orfium.atlassian.net/wiki/spaces/FE/pages/927039566/Commits+-+How+we+contribute)

### Pull Request

When you're finished with the changes, create a pull request, also known as a PR.  
- Fill in the "Ready for review" template so that we can review your PR. This template helps reviewers understand your changes as well as the purpose of your pull request.   
- Don't forget to link any JIRA ticket on the PR header - if you are solving one.  
Once you submit your PR, a member will review it. We may ask questions or request additional information.  
- We may ask for changes to be made before a PR can be merged. PR rules of the team can be found [here](https://orfium.atlassian.net/wiki/spaces/FE/pages/924254280/Pull+Requests)

If you are NOT part of the FE team as we need to keep align with all the changes that happens we will be responsible for the PR merge. 
If you are the owner and part of the FE team you are allowed to merge your PR when it gets the approvals neccessary.

### Your PR is merged!

Congratulations :tada::tada:

---
# QA
### Setup
First, you should install the (dev) requirements of the project. Usually, it's a file called `requirements_dev.txt`. The pre-commit requirement should be included there.  
Next, make sure to [install "pre-commit"](https://pre-commit.com/#3-install-the-git-hook-scripts) locally. Running `pre-commit install` should be enough.
### Add your change locally
1. Create a branch from master(make sure you pull the latest changes). A good convention for the branch name is to incude the Jira ticket eg. "QA-17/create-new-functionality".
2. After coding your changes create one or more commits. The commit messages should follow the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#summary) format. Each commit should trigger the "pre-commit" checks. If it doesn't there is something wrong with the configuration.
3. In case the "pre-commit" hooks made any changes(autofixes) you need to re-add the changed files (`git add <file>`) and commit again.
4. Once you're finished push your local branch to the remote repository with `git push origin <branch-name>`

### Pull Request
Go to the GitHub repository and open a pull request.  
Usually, there are scripts that auto-assign some reviewers. You should **always** choose as assignees the ones that are more relevant to your changes (eg. have good knowledge of the specific framework, have worked again on something similar, know the codebase well, etc)
- Please fill out the description from the PR template provided.
- Don't forget to link any JIRA ticket on the PR header or any [GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue) - if you are solving one.
- Please test your changes both locally and on Jenkins (using the test pipelines) before asking for a review. 

You're good to go! 
