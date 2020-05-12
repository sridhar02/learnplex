---
id: prerequisites
title: Prerequisites
sidebar_label: Prerequisites
---

1. [Node](https://nodejs.org/en/download/) >= 10.x
    ```sh
    # To check if node is installed and find its version, run
    node -v
    ```
    > If you face problem updating your node then you might need a Node version manager tool like [nvm](https://github.com/nvm-sh/nvm)
1. [Yarn](https://classic.yarnpkg.com/en/docs/install) >= 1.5
    ```sh
    # To check if yarn is installed and find its version, run
    yarn -v
    ```
    > We only use Yarn as our official Node package manager, and so we request you to use `Yarn` instead of `npm` and commit `yarn.lock` file.
1. [PostgresQL](https://www.postgresql.org/download/) >= 12.x
    ```sh
    # To check if postgres is installed and to find its version, run
    psql -V
   
    # To check if postgres is running, run
    pg_isready
    # You should see something like
    > /tmp:5432 - accepting connections
    ```
1. [Redis](https://redis.io/download)
    ```sh
    # To check if redis is running, run
    redis-cli ping
    # You should get back 
    > PONG
    ```
