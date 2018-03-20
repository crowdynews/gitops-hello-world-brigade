# GitOps Hello World v2

Second iteration of the Hello world REST API used to demonstrate a more decoupled GitOps workflow.

This workflow uses [Google Container Builder](https://cloud.google.com/container-builder/) as the
CI system to build Docker images and push them to [Google Container Registry](https://cloud.google.com/container-registry/).

## Infrastructure Config

* [Staging](https://github.com/crowdynews/gitops-hello-world-infra-staging-v2)

## Running locally

```
npm i && npm start
```

The following env vars can be set:

| PROPERTY   | REQUIRED | DEFAULT VALUE                   |
| ---------- | -------- | ------------------------------- |
| `API_HOST` | no       | `0.0.0.0` set in `./src/app.js` |
| `API_PORT` | no       | `8888` set in `./src/app.js`    |

## Google Identity & Access Management Roles

GCP IAM requires `[PROJECT_ID]@cloudbuild.gserviceaccount.com` to have the following roles:

* Cloud Container Builder
