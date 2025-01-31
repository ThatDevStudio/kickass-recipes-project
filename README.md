# Kickass Recipes Project

## Overview

“Kickass Recipes” is a fullstack application which can be used for managing recipes along with quality-of-life features around automatic servings calculations, nutritional information, and shopping lists. The goal of this project is to build a useful application while learning many of the core skills required for fullstack development.

## Components

- A react + typescript frontend using popular libraries like axios for http requests, tailwindcss for styling, shadcn/ui for generating accessible and  user-friendly components, React Router for routing, and Tanstack Query for global state and cache management.
- A flask + python backend leveraging the full power of python types while using popular libraries like requests for integrating with external APIs, SQLAlchemy as the primary database ORM, Alembic for managing database migrations, Pydantic for environment management and types marshalling, and Authlib for a fully-featured authentication layer.
- OpenAPI for a solid contract between the frontend and the backend
- GitHub actions for development of CI/CD pipelines for a developer-friendly ecosystem
- Docker and Docker compose for seamless development and deployment to production environments
- AWS services like IAM, Secrets Manager, ECR and ECS for hosting full-stack, containerized applications
- Terraform for managing AWS resources

## Modules

The following is a rough layout of the project in terms of modules and what they attempt to accomplish. Treat each module as lasting between 1-2 weeks depending on the complexity. We will chat about each in our Friday sessions while leaving the bulk of the build as “homework”.

### Module 1 - Project initialization

We will start with the creation of the project’s components in GitHub, downloading necessary tooling for local development, and producing our first commit!
Backend & database setup
Next, we will focus on setting up the boilerplate backend and our databases. This will enable us to begin development of the API. We will build out our first couple of endpoints and initialize our database with a few tables. Our goal will be to create basic CRUD endpoints for the core models and persist those changes to the database, leveraging tools like Beekeeper and Postman for assistance.

### Module 2 - Frontend & API contract setup

Next, we will focus on the setup of the frontend and begin developing our API contract as a guide for backend development. We will build out a simple page to list recipes which are stored in the backend and specific pages for each recipe with routing. Our goal will be to view and create recipes on the frontend and have those pages interact with the backend, leveraging tools like React Query and React Router.

### Module 3 - AWS Deployment

At this middle point in the project, we will deploy our very simple application to AWS. We will build our Docker files and initialize Terraform to manage our AWS resources. Finally, we will stand up our AWS resources and deploy our project images to those via Github actions

### Module 4 - Authentication

This entire module will focus on authentication. How to authenticate on the frontend and authorize users to roles on the backend, which can be propagated throughout the API endpoints and interaction with the database. We will also create functionality on the frontend for users to login, logout, and view profiles. Finally, we will create user-settings which can be applied at every login.

### Module 5 - Wave 1 of new features: Servings Calculations

We will create a new servings calculations feature. The first wave of new features will focus on learning how to collaborate in GitHub, review and issue PRs appropriately, and to build in linting and type checking into our pipelines to ensure our applications have a consistent baseline in quality. We will discuss new components on the frontend and state management in React.

### Module 6 - Wave 2 of new features: Shopping Lists

We will create a new feature to allow users to create, share, and manage shopping lists. We will focus on building these new pages on the frontend, building new API endpoints on the backend, and finally how to develop new tables and migrate our existing database with the new tables.

### Module 7 - Wave 3 of new features: Nutritional Details

As the final module in this project, we will integrate with external APIs to gather nutritional information for recipes which can be viewed with the recipe, scaled to the appropriate serving size (see 6). This will involve managing development and production keys for external APIs and the development of a cacheing layer on the backend.
