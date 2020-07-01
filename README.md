# Mobile: React Native Concepts

Example GitHub Repository Mobile Application that uses the Repository API, the backend project we have developed earlier.

## Usage

After cloning the repo, you should run this command in order to have everything initialized for development:

````
yarn
````

or 

````
npm install
````

Next, issue these commands if you are developing an Android app (notice that jetifier is enabled by default):

````
yarn add jetifier -D
yarn run jetify
yarn run react-native run-android
````

or

````
npm install --save-dev jetifier
npx jetify
npx react-native run-android
````

If you are developing an iOS app, you must enter the ``ios/`` directory and install all its pods, as in:

````
pod install
````

Alternatively, you can just run tests:

````
yarn test
````

or 

````
npm test
````

That's it!

## Tips

If you run an iOS app under emulator, you are all just set since you install XCode. If you run  Android apps though, you must "proxy" tcp under port ``3333`` before running it, like this:

````
adb reverse tcp:3333 tcp:3333
````