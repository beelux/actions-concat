
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
