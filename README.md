# Deploy Strapi with Porter
This is a quickstart repository you can fork to deploy Strapi to Kubernetes on AWS/GCP/DO with Porter. This sample repository uses PostgresDB by default. Modify the files in `/app/config/env/production` to customize your database settings.

# Quick Deploy
1. Create an account on [Porter](https://dashboard.getporter.dev).
2. [One-click provision a Kubernetes cluster](https://docs.getporter.dev/docs/getting-started-with-porter-on-aws) in a cloud provider of your choice, or [connect an existing cluster.](https://docs.getporter.dev/docs/cli-documentation#connecting-to-an-existing-cluster)
3. Fork this repository.
4. From the [Launch tab](https://dashboard.getporter.dev/launch), navigate to **Web Service > Deploy from Git Repository**, select the forked repository and `Dockerfile` in the root directory.
5. Configure the port to `1337`, add environment variable `NODE_ENV=production`, and set resources to the [recommended settings](https://strapi.io/documentation/developer-docs/latest/setup-deployment-guides/deployment.html#general-guidelines) (i.e. 2048Mi RAM, 1000 CPU).
6. Hit Deploy!

# Development
To develop, clone this repository to your local environment and run `yarn install && yarn develop;` from the `app` directory.

# Questions?
Join the [Porter Discord community](https://discord.gg/FaaFjb6DXA) if you have any questions or need help.