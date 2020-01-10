
# Multi-repo approach: deploying scratch-vm and -gui forks using Travis CI

## Set up for scratch-vm

## Set up for scratch-gui

1. Update package.json to reference your GitHub branch's version of scratch-vm
2. Create a `GH_TOKEN` [following these steps](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line#creating-a-token)
    - Give it only `public_repo` permissions
2. Enable builds for your

# Monorepo Approach

https://github.com/MrYsLab/s3onegpio is a nice example of using a monorepo approach, keeping scratch-vm and -gui in the same directory.

- Pros: new blocks can be added to both projects at the same time
- Cons: lose history of the sub-directories, harder to push changes back upstream
