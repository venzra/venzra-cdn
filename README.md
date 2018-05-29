# Venzra CDN

Content delivery for assets used on Venzra websites

[![CircleCI](https://circleci.com/gh/sysen-limited/venzra-cdn.svg?style=svg&circle-token=ddcd30a15ba817e8740c542eac35e7c425249e13)](https://circleci.com/gh/sysen-limited/venzra-cdn)

### Deployment

Deployment occurs via CircleCI on commit to master, the following environment variables are required

| variable | example | description |
| :--- | :--- | :--- |
| DEPLOY_CERT | arn:aws:acm:us-east-1:xxxxxxxxxxxx | AWS certificate ARN, certificate must exist on US-EAST-1 |
| DEPLOY_URI | cdn.venzra.com | The domain for which to create this CDN |
| DEPLOY_STACK | cdn-venzra | The name for AWS to use to reference this environment |
