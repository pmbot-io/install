<p align="center">
  <a href="https://pmbot.io">
    <img alt="Pmbot" src="https://raw.githubusercontent.com/pmbot-io/public-branding/master/logo/logo-horizontal.svg" width="300"/>
  </a>
</p>
<h1 align="center">Install</h1>

This project is meant to help users deploy the self-hosted version of Pmbot.

The deployment relies on [Docker](https://docs.docker.com/) and [Docker Compose](https://docs.docker.com/compose/).

## Deployment

### Clone

```shell script
git clone https://github.com/pmbot-io/install.git pmbot
cd pmbot
```

### `.env` file

Create an `.env` file by copying `.env.example`:
```shell script
cp .env.example .env
``` 

This file contains variables needed by the `docker-compose.yml`.
You may modify it to suit your needs.

### Docker Compose

You can then launch Pmbot with the command:

```shell script
docker-compose up --detach
```

## Update

We strongly recommend that you avoid modifying versioned files as much as possible to ease the update process.
If your use case cannot be covered with the `.env` file, feel free to open an issue.

```shell script
git pull
docker-compose pull
docker-compose up --detach
```

## Documentation

See our [documentation](https://docs.pmbot.io/core/installation) for more information on environment variables.
