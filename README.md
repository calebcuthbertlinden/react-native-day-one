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

## Styling
Most React Native components accept a style prop that accepts a JavaScript object as its value. For more details, see Styling in React Native.

React Native uses the same color format as the web. It supports hex triplets (this is what #fff is), rgba, hsl, and named colors, such as red, green, blue, peru, and papayawhip. For more information, see Colors in React Native.

## 