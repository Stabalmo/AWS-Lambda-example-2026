# AWS-Lambda-examples — AWS Lambda + API Gateway (HTTP API) Examples (SAM, Python)

This repository provides **AWS Lambda examples** with **API Gateway HTTP API**, a **Lambda Authorizer (Bearer token)**, and **DynamoDB**—built and deployed using **AWS SAM**.

## Start here (Step-by-step guide)

**[Open the complete AWS Lambda + API Gateway guide](./AWS-Lambda-API-Gateway-Guide.md)**

## What you get
- **Endpoints**: `GET /health` (public), `POST /items`, `GET /items/{id}`, `DELETE /items/{id}` (authorized)
- **Auth**: Lambda authorizer reads token from **SSM Parameter Store**
- **Persistence**: DynamoDB table for items
- **Ops**: CloudWatch Logs + X-Ray enabled

## Repo files
- `template.yaml`: SAM template (API Gateway, Lambdas, DynamoDB, permissions)
- `src/app.py`: API Lambda handler
- `src/authorizer.py`: Lambda authorizer
- `scripts/integration_test.sh`: simple integration test script
- `AWS-Lambda-API-Gateway-Guide.md`: full deployment + troubleshooting guide

## Legacy guide filename
If you have links/bookmarks to the old guide name, it’s kept as a redirect:
- `GUIDE_INSTRUCTION.md`
