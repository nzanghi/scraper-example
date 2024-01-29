# Prerequisites

## Things to Download

Before you start downloading things, if you do not know what your computer's architecture is, you can check with the following command using Powershell:

```shell
wmic OS get OSArchitecture
```

1. [Visual Studio Code](https://code.visualstudio.com/download)

   Use this for modifying code. Highly recommend [using the command line interface (cli) for it](https://code.visualstudio.com/docs/editor/command-line#_launching-from-command-line)

2. [NodeJS](https://nodejs.org/en)

   This will execute and run your code. Download Long Term Support (LTS) version.
   You will know you installed it correctly by typing the following command in Powershell, and seeing the version output:

   ```shell
   node --version
   # v20.11.0 / current LTS version
   ```

3. [pnpm](https://pnpm.io/installation#on-windows)

   Use this for downloading packages from https://www.npmjs.com
   You will know you installed it correctly by typing the following command in Powershell, and seeing the version output:

   ```shell
   pnpm --version
   # 8.15.1 / current LTS version
   ```

4. [git](https://git-scm.com/download/win)

   Use this for actually copying the code from here! You can clone this repository to a local directory on your computer with the following command:

   ```shell
   git clone
   ```

If you do NOT see the output above when you type the commands in Powershell, you should take a look at your [PATH](https://learn.sparkfun.com/tutorials/configuring-the-path-system-variable/all) environment variable

# Setting up

1. Clone this repo

```shell
git clone repo
```

2. Use `pnpm` to install dependencies

```shell
pnpm i
```

3. Launch the scraper

This command uses `pnpm` to lookup the `start` script inside of the `package.json` file

```shell
pnpm start
```

This command will use `node` directly to launch the code you've written in `index.js`

```shell
node index.js
```

# Updating Code

The code written in `index.js` utilizes [Puppeteer](https://pptr.dev/) a library meant to automate browser interactions. Read the docs to find out how to use it!
