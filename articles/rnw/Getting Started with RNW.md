# Getting Started with React Native Web

## Using Expo

## Setup

:::image type="content" source="misc/expo init.JPG" alt-text="Expo init":::

## Publishing

We chose `Github-Pages` to host our site. According to [expo doc](https://docs.expo.io/distribution/publishing-websites/#github-pages):

- If you haven't done so:

```bash
git init
git remote add origin <YOUR_GITHUB_PAGES_URL>
yarn add -D gh-pages
```

- Add the following to your package.json:

```bash
/* package.json */
{
    "homepage": "http://evanbacon.github.io/expo-gh-pages",
    "scripts": {
        "deploy": "gh-pages -d web-build",
        "predeploy": "expo build:web"
    }
}
```

- Finally deploy with:

```bash
yarn deploy
```
