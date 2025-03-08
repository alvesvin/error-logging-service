# Error Loggin Service Architecture

## Customer Questions

I have previous knowledge from the requirements document and I'm supposing that this service is similar to Sentry, DataDog, etc.

### What kind of services would you like to support? Frontend, backend, mobile, which languages?

Customer> I'd like to support both frontend and backend in the NodeJS ecosystem as an MVP but I'm willing to expand to other languages and environments.

### Do you know other services that is comparable to this one and that you would like to take inspiration from?

Customer> I know Sentry is a very popular service and I like their interface and ease of use.

### Who are your intended users?

Customer> I want this service to be used by developers of any sized company, globally.

### What is your expected time frame for this project?

Customer> I'm looking to release this MVP in the next 6 months.

Based on the the questionaire, I'm going to propose a reduced architecture that will be used for the MVP.

## Architecture Overview

### Tech Stack

- NestJS: Leading backend framework for NodeJS, a lot of pre-built components and well-thought patterns.
- NextJS: Leading frontend framework, powerful, flexible and industry standard.
- PostgreSQL: A powerful, flexible, open source, relational database. Gives us a room for improvements and has a lot of features.
- Kubernetes: Industry standard container orchestration platform. Awesome for deploying and scaling.
- Docker: For building and deploying containers.
- AWS: For cloud solutions. Cheaper than alternatives, easier to manage, and industry leading.
- NGINX: For load balancing and reverse proxying.

### Libs and third-party services

- Clerk: for instant authentication and security
- Tanstack Query: for data fetching management
- WebSocket: for real-time data streaming
- TailwindCSS: for styling
- Resend: email service
- shadcn/ui: for UI components
- Own Service: for error logging

### Architecture Diagram

![Architecture Diagram](https://github.com/plugify/error-logging-service/blob/master/docs/images/architecture.png)
