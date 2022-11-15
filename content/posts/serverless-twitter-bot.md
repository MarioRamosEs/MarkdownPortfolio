---
title: Serverless Community Twitter Bot
date: 2022-10-25
published: true
tags: ["Personal Project", "Azure", ".NET"]
series: false
cover_image: ./images/ServerlessTwitterBotHeader.png
canonical_url: false
description: "Twitter bot hosted Azure using Functions, CosmosDB, KeyVault and Vue"
---

Serverless Twitter bot that each 12h, tweets a random sentence from a list of sentences. It also allows any user to suggest their own ones.

Hosted in Azure using Functions, CosmosDB, KeyVault, Static Web Apps and Vue

[Web page](https://purple-bush-0eb409903.2.azurestaticapps.net/)

[@GigachadBot\_ in Twitter](https://twitter.com/GigachadBot_)

## Backend Architecture
<div align="center">
  <img style="width: 100%; max-width: 800px;" src="../images/serverlessTwitterBot/backend-arch.png">
</div>

The backend consist of a solution based in **clean architecture, CQRS pattern with MediatR** and a CosmosDB database managed by Entity Framework. The solution is divided in 4 projects:

### ServerlessCommunityTwitterBot
Contains different Azure functions, of which only tree are used in production

  - **PublishTweet**: Function that tweets a random sentence from the database, and updates the last tweet date
  - **CreatePendingSentence**: Function that creates a new pending sentence in the database, and then sends a email to the admin with links to approve or reject the sentence
  - **ResolvePendingSentence**: Function that resolves a pending sentence, if its approved it will be added to the database, if its rejected it will be deleted

<div align="center">
  <img style="width: 100%; max-width: 800px;" src="../images/serverlessTwitterBot/functionExample.png">
</div>    

### Infrastructure
Contains the abstractions of any external dependencies
<div align="center">
  <img style="width: 100%; max-width: 800px;" src="../images/serverlessTwitterBot/insfrastructureServices.png">
</div>

### Application
Contains the application logic, the commands and queries of the CQRS pattern are defined here.

Each command or query goes through pipelines that run model validations using FluentValidation, and handle any unhandled exceptions

<div align="center">
  <img style="width: 100%; max-width: 800px;" src="../images/serverlessTwitterBot/commandExample.png">
</div>

### Domain
Contains the entities, the custom excepctions and the interfaces of the services

[Backend GitHub Link](https://github.com/MarioRamosEs/ServerlessCommunityTwitterBot)

## Frontend Architecture
The project needed a small form so that users could suggest their sentences, so I created a simple webpage in [Vue 3](https://vuejs.org/), using [Vite](https://vitejs.dev/) and the great UI library [Vuetify 3](https://next.vuetifyjs.com/)

[Take a look at the page](https://purple-bush-0eb409903.2.azurestaticapps.net/)

[and the code in GitHub](https://github.com/MarioRamosEs/ServerlessCommunityTwitterBotVue)
<div align="center">
  <img style="width: 100%; max-width: 500px;" src="../images/serverlessTwitterBot/sendSentence.png">
</div>

## Azure
The project is hosted in Azure, using the following services:
  - **Azure Functions**: To host the backend functions in a consumption plan
  - **Azure CosmosDB**: To store the sentences
  - **Azure KeyVault**: To store the secrets
  - **Azure Static Web Apps**: To host the frontend

Services are linked to their repositories and updated using GitHub Actions

<div align="center">
  <img style="width: 100%; max-width: 500px;" src="../images/serverlessTwitterBot/azureServices.png">
</div>