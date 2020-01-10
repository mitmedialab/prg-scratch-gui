
# Multi-repo approach: deploying scratch-vm and -gui forks using Travis/CircleCI

## Set up for scratch-vm

scratch-vm is built using Travis CI. Travis is free for public repositories.



## Set up for scratch-gui

scratch-gui is built using CircleCI, since it seems like the latest direction planned to be used upstream.

1. Update `.circleci/config.yml` to reference your GitHub branch's version of `scratch-vm`
1. Enable builds for your fork at circleci.com (since the repo already has a `.circleci/config.yml`, you can ignore that part)
1. Create a `GH_TOKEN` [following these steps](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line#creating-a-token)
    - Give it only `public_repo` permissions

# Monorepo Approach

https://github.com/MrYsLab/s3onegpio is a nice example of using a monorepo approach, keeping scratch-vm and -gui in the same directory.

- Pros: new blocks can be added to both projects at the same time
- Cons: lose history of the sub-directories, harder to push changes back upstream
