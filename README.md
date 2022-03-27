# DigitalOcean Static App

This repository contains the files needed to serve a static app and deploy via DigitalOcean [App Platform](https://docs.digitalocean.com/products/app-platform/). However,
the main objective is to use Terraform to deploy the App using my repository [terraform-digitalocean](https://github.com/kwame-mintah/terraform-digitalocean).

## Development

### Dependencies
- DigitalOcean account
- pre-commit

## Usage

To deploy the static app using Terraform, please see my repository [terraform-digitalocean](https://github.com/kwame-mintah/terraform-digitalocean).

Alternately, you can use the button below to deploy the app to your DigitalOcean account:

[![Deploy to DO](https://www.deploytodo.com/do-btn-blue-ghost.svg)](https://cloud.digitalocean.com/apps/new?repo=https://github.com/kwame-mintah/digitalocean-static-app/tree/master)

Please note with the following configuration for the app:
* Pushing to the 'master' branch will trigger the app to be built again,
* No environment variables need to be set for the app to work.

You will be charged in DigitalOcean if you're deploying more than 3 static sites.

### Pre-Commit hooks

Git hook scripts are very helpful for identifying simple issues before pushing any changes. Hooks will run on every commit automatically pointing out issues in the code e.g. trailing whitespace.

To help with the maintenance of these hooks, [pre-commit](https://pre-commit.com/) is used, along with [pre-commit-hooks](https://pre-commit.com/#install).

Please following [these instructions](https://pre-commit.com/#install) to install `pre-commit` locally and ensure that you have run `pre-commit install` to install the hooks for this project.

Additionally, once installed, the hooks can be updated to the latest available version with `pre-commit autoupdate`.
