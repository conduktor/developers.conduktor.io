# Conduktor API docs

## Deployment overview

- [URL](developers.conduktor.io)
- [Vercel project](https://vercel.com/conduktor/developers-conduktor-io)

## Updating API docs

API docs live on `host:8888` of the deployed Gateway/Console and are also published to: [Gateway API](https://developers.conduktor.io/?product=gateway) and [Console API](https://developers.conduktor.io/?product=console) docs.

To update the public docs:

1. Copy the latest open API yaml files from the `conduktor-proxy` repo based on the version:
    - Gateway v1
    - Gateway v2
    - Console
2. Paste the yaml files to **openapi** and rename as required.
3. Add the new version to **openapi/manifest.json**.
