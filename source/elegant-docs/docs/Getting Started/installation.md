---
title: Installation
slug: /
sidebar_position: 1
sidebar_label: Installation
---

# Installation

- [Meet Elegant](#meet-elegant)
    - [Why Elegant?](#why-elegant)
- [Your First Elegant Project](#your-first-elegant-project)
- [Initial Configuration](#initial-configuration)
    - [Environment Based Configuration](#environment-based-configuration)

<a name="meet-elegant"></a>

## Meet Elegant

 Elegant is a utility-first CMS framework for rapidly building expressive and elegant static content web applications. A CMS framework provides a structure and a starting point for creating a beautiful application, blog, or documentation website. 


<a name="why-elegant"></a>

### Why Elegant?

There are a variety of tools and frameworks available to you when building a frontend application. However, we believe Elegant is the best choice for building amazing, and elegant web applications.

<a name="your-first-elegant-project"></a>

## Your First Elegant Project

Before creating your first Elegant project, you should ensure that your local machine has [Node and NPM](https://nodejs.org) installed.

The next step is to intall the Elegant CLI tool via npm.

```nothing
npm install elegant-cli --save-dev
```

After you have installed the Elegant CLI tool, you may create a new Elegant documentation project via the NPM `npx elegant-docs-init` command:

```nothing
npx elegant-docs-init
```

After the project has been created, install the required Node packages, and start Elegant's local development server using npm:

```nothing
npm install

npm run start
```

Once you have started the Elegant development server, your application will be accessible in your web browser at `http://localhost:3000/docs`.

To stop the Elegant development server, press the `ctrl` and `c` keys together in the terminal:

```nothing
ctrl + c
```

<a name="initial-configuration"></a>

## Initial Configuration

Elegant needs almost no additional configuration out of the box. You are free to get started developing!

<a name="environment-based-configuration"></a>

### Environment Based Configuration

Since many of Elegant's configuration option values may vary depending on whether your application is running on your local machine or on a production web server, many important configuration values are defined using the `.env` file that exists at the root of your application.

Your `.env` file should not be committed to your application's source control, since each developer / server using your application could require a different environment configuration. Furthermore, this would be a security risk in the event an intruder gains access to your source control repository, since any sensitive credentials would get exposed.

> **Note**  
> For more information about the `.env` file and environment based configuration, check out the full [configuration documentation](/docs/configuration#environment-configuration).