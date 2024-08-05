#  TopFold

This is a Next.js application that uses Contentful as the headless CMS to manage and deliver content.

## Get Started with Next.js

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).
Once install dependencies, run the development server:

```bash
npm i
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Content Management with Contentful

Start by [signing up for a Contentful account](https://www.contentful.com/sign-up/). This will allow you to create and manage your content within the Contentful platform.

### Contentful CLI

This project includes the Contentful CLI as a development dependency. You can run Contentful CLI commands using npm scripts. Below is an example command and a detailed explanation of its components:

```bash
npm run contentful -- <command>
```

- `npm run contentful`: Runs the `contentful` script from `package.json`, invoking the Contentful CLI from `node_modules` without needing a global install.
  
- `--`: This double dash is a separator that tells npm to pass any subsequent arguments directly to the Contentful CLI.

For example, the following command lists all the commands related to the Contentful space:

```bash
npm run contentful -- space --help
```

### Contentful Login

Log in to your contentful using the following command

```bash
npm run contentful -- login  
```

This command prompts you to authorize the login in a browser. Once completed, paste the access token ([Contentful Management Token](https://www.contentful.com/developers/docs/references/content-management-api/#/introduction/authentication)) into the Contentful CLI prompt. **Important:** Do not commit or share this management token, as it grants write access to your Contentful account.

```bash
A browser window will open where you will log in (or sign up if you don’t have an account), authorize this CLI tool and paste your CMA token here:

? Continue login on the browser? Yes
? Paste your token here: *******************************************

Great! You've successfully logged in!
```
