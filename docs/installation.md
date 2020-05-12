---
id: installation
title: Installation
sidebar_label: Installation
---

## Running Learnplex locally
1. Fork the [repository](https://github.com/coderplex/learnplex)
1. Clone the forked repository
    ```sh
    git clone <your-forked-repo-url>
    ```
1. Move to the repo folder
    ```sh
    cd learnplex
    ```
1. Install dependencies
    ```sh
    yarn
    ```
1. Start the development server
    ```sh
    yarn dev
    ```
    You can view your application at [localhost:3000](http://localhost:3000) in your browser

## Running Learnplex-Backend locally
1. Fork the [repository](https://github.com/coderplex/learnplex-backend)
1. Clone the forked repository
    ```sh
    git clone <your-forked-repo-url>
    ```
1. Move to the repo folder
    ```sh
    cd learnplex-backend
    ```
1. Create .env file from .env.sample
    ```sh
    cp .env.sample .env
    ```
1. Follow the instructions at [creating-an-oauth-app](https://developer.github.com/apps/building-oauth-apps/creating-an-oauth-app/) to create an oauth app.
    > Set the Authorization callback URL to `http://localhost:4000/auth/github/callback`
1. Now visit [Developer Settings](https://github.com/settings/developers) and open your newly created application in OAuth Applications. 
1. Copy the `Client ID` and `Client Secret` from here and set them in your `.env` file
1. Create `coderplex` db
    ```sh
    createdb coderplex
    ```
1. Install dependencies
    ```sh
    yarn
    ```
1. Start the development server
    ```sh
    yarn dev
    ```
    You can view your application at [localhost:4000](http://localhost:4000) in your browser
1. You can access Graphql Playground at [localhost:4000/graphql][http://localhost:4000/graphql] in your browser

