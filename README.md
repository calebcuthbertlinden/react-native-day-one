# React Native
Learn once, write anywhere.
[https://reactnative.dev/](reactnative.dev)

We believe that the best way to experience React Native is through a Framework, a toolbox with all the necessary APIs to let you build production ready apps.
> In comes [https://expo.dev/](Expo) - Expo provides features like file-based routing, high-quality universal libraries, and the ability to write plugins that modify native code without having to manage native files.

[Getting started](https://reactnative.dev/docs/environment-setup)

## Install Node and nvm
```
# Install nvm (if not already installed)
curl -fsSL https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash

# Restart terminal or run
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"

# Install latest LTS version of Node.js
nvm install --lts

# Verify installation
node -v
npm -v
npx -v

```

## Create expo app
```
npx create-expo-app@latest myApp
cd myApp
npx expo start
```

## app/index.tsx
It is the entry point of our app and executes when the development server starts.

## Chapter 1 - Styling
Most React Native components accept a style prop that accepts a JavaScript object as its value. For more details, see Styling in React Native.

React Native uses the same color format as the web. It supports hex triplets (this is what #fff is), rgba, hsl, and named colors, such as red, green, blue, peru, and papayawhip. For more information, see Colors in React Native.

## Chapter 2 - Navigation
Expo Router is a file-based routing framework for React Native and web apps. It manages navigation between screens and uses the same components across multiple platforms. To get started, we need to know about the following conventions:

### Basics
- **app directory**: A special directory containing only routes and their layouts. Any files added to this directory become a screen inside our native app and a page on the web.
- **Root layout**: The app/_layout.tsx file. It defines shared UI elements such as headers and tab bars so they are consistent between different routes.
- **File name conventions**: Index file names, such as index.tsx, match their parent directory and do not add a path segment. For example, the index.tsx file in the app directory matches / route.
- A **route** file exports a React component as its default value. It can use either .js, .jsx, .ts, or .tsx extension.
- Android, iOS, and web share a unified navigation structure.

> More [information](https://docs.expo.dev/router/introduction/) about routes and navigation

### What is <Stack>?
A stack navigator is the foundation for navigating between different screens in an app. On Android, a stacked route animates on top of the current screen. On iOS, a stacked route animates from the right. Expo Router provides a Stack component to create a navigation stack to add new routes.

### <Link>
We'll use Expo Router's Link component to navigate from the /index route to the /about route. It is a React component that renders a <Text> with a given href prop.

### Bottom navigation bar
Inside (tabs)/_layout.tsx, add a Tabs component to define the bottom tab layout:
![alt text](<navigation.png>)

## Chapter 3 - Build a screen
