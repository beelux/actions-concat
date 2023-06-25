# Actions Concatentation

This repo serves as a basic demo of how one can use GitHub Actions to generate files and commit them back.

Following is a basic introduction to GitHub Actions, but this serves more as a demo. See the workflow file to understand what happens.

## Usage

### Introduction

GitHub Actions is an product offered by GitHub that allows for *general **automation***:

- respond to Issues
- run tests on Pull Requests
  - syntax
  - end-to-end tests
- Building
  - tagging the lastest `main` commit and publishing a `dev` release with binaries
  - building binaries when a new release is created
- Deploying
  - deploying to a staging environment (e.g. netlify) when commits are made to `staging`
  - deploying to production when commits are made to `main`

You can effectively run automated computation, related to your project, on GitHub-provided or self-hosted machines.

GitHub currently provides various runners:

- Linux
- Windows
- macOS

### Basics

- Each file is a **workflow**
  - which is a set of **jobs**
    - which is a set of **steps**

- Each **job** is run in a separate VM (fresh runner)
- **Steps** can be commands or *pre-made marketplace actions*
- **Secrets** are stored in the repo's settings
  - part of the workflow's "environment variables"
- **Artifacts** are files that can be passed between jobs
  - e.g. build artifacts
- **Events** trigger workflows, e.g.:
  - `workflow_dispatch` (manual trigger)
  - `push`
  - `pull_request`
  - ...

### Pricing

- Self-hosted runners are free.

- Public repositories on GitHub are free to use GitHub Actions.
- Private repositories must pay for GitHub Actions, but e.g.:
  - For `Free` users: 2'000 free minutes per month

Note that this information is bound to change at any moment. Please refer to the official GitHub website.

## Various

This could be something additional.

### `cat`

The `cat` command is widely known and used, but very few know that this is what happens inside of your operating system when using it:

![cat](/additional/cat.png)

### Dog

Cats are not the only ones using computers. As you might know from Internet lore:
> On the Internet, nobody knows you're a dog.

Indeed, anyone you talk to online could be as nice as this dog:
![dog](/additional/dog.png)

## License

I cannot give a license to this project as it is closer to learning material than a project.

The images are licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).
