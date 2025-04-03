# React Native
Learn once, write anywhere.
[https://reactnative.dev/](reactnative.dev)

We believe that the best way to experience React Native is through a Framework, a toolbox with all the necessary APIs to let you build production ready apps.
> In comes [https://expo.dev/](Expo) - Expo provides features like file-based routing, high-quality universal libraries, and the ability to write plugins that modify native code without having to manage native files.

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