# GitOps Hello World v2
Second iteration of the Hello world REST API used to demonstrate a more decoupled GitOps workflow.

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
