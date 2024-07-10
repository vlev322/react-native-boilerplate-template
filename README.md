# react-native-boilerplate-template

[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

It is a template that you can clone and reuse for every project. It is starting point for React Native application.

## React Native Boilerplate

consist of:

- "react-native": "0.73.1",
- "@react-native-masked-view/masked-view": "^0.3.1",
- "@react-navigation/bottom-tabs": "^6.5.11",
- "@react-navigation/material-top-tabs": "^6.6.5",
- "@react-navigation/native": "^6.1.9",
- "@react-navigation/native-stack": "^6.9.17",
- "@react-navigation/stack": "^6.3.20",
- "react": "18.2.0",
- "react-native-gesture-handler": "^2.14.0",
- "react-native-pager-view": "^6.2.3",
- "react-native-safe-area-context": "^4.8.2",
- "react-native-screens": "^3.29.0",
- "react-native-tab-view": "^3.5.2",
- "react-native-vector-icons": "^10.0.3"

## Requirements

Node 18 or greater is required. Development for iOS requires a Mac and Xcode 10 or up, and will target iOS 11 and up.

You also need to install the dependencies required by React Native.
Go to the [React Native environment setup](https://reactnative.dev/docs/environment-setup), then select `React Native CLI Quickstart` tab.
Follow instructions for your given `development OS` and `target OS`.

## QUICK START

To create a new project using the boilerplate simply run :

```
npx react-native@latest init MyApp --template github:vlev322/react-native-boilerplate-template
```

note: replace `MyApp` with your desired App name.

Assuming you have all the requirements installed, you can run the project by running:

- `yarn start` / `npm start -- -- reset-cache`  to start the metro bundler, in a dedicated terminal
- `npx react-native run-ios` / `npx react-native run-android`  to run the *platform* application (remember to start a simulator or connect a device)

## List of Q & A

#### I got error `Error: spawn ./gradlew EACCES` when run `npx react-native run-android`

Run this command `chmod 755 android/gradlew` from your root project directory

#### I got error `Error: SDK location not found. Define location with sdk.dir in the local.properties file or with an ANDROID_HOME environment variable.`

- Go to your Project -> Android
- Create a file local.properties
- Open the file
- Paste your Android SDK path depending on the operating system:

  - Windows:
    sdk.dir=C:\\Users\\`USERNAME`\\AppData\\Local\\Android\\sdk
  - Linux or MacOS
    sdk.dir=/Users/`USERNAME`/Library/Android/sdk

- Replace `USERNAME` with your PC username
