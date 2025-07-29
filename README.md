# Conduktor API docs

For main docs, see [docs repo](https://github.com/conduktor/conduktor-docs).

## Deployment overview

- [URL](developers.conduktor.io)
- [Vercel project](https://vercel.com/conduktor/developers-conduktor-io)

## Automated updates

These API docs are automatically updated by the [`update-api-docs` action in the `conduktor-actions` repo.](https://github.com/conduktor/conduktor-actions/tree/main/update-api-docs)

The action will perform the manual steps below, copying the openapi yaml files from each repo.

## Manual updates

API docs live on `host:8888` of the deployed Gateway/Console and are also published to: [Gateway API](https://developers.conduktor.io/?product=gateway) and [Console API](https://developers.conduktor.io/?product=console) docs.

To update the public docs:

1. Copy the latest open API yaml files from the `conduktor-proxy` or `console-plus` repo based on the version:
   - [Gateway v1](https://github.com/conduktor/conduktor-proxy/blob/main/proxy/src/main/resources/gateway-API.yaml)
   - [Gateway v2](https://github.com/conduktor/conduktor-proxy/blob/main/api-definition/src/main/resources/openapi.yaml)
   - [Console](https://github.com/conduktor/console-plus/blob/main/modules/consoleplus/app/src/main/resources/public-api-doc.yaml)
2. Paste the yaml files to the relevant directory within **openapi** and rename as required with the version number of the latest update.
3. Add the new version number to **openapi/manifest.json**.
