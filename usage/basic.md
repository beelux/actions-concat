
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
