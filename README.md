<h2 align='center'>harry potter characters app</h2>




### install dependencies

```bash
npm install
# or delete the package-lock.json and use yarn
yarn install
```

### start dev server

```bash
expo start
# or
npx expo start
```

### build

use the EAS cli to build the app, APK for testing and AAB for submission to the play store

```bash
# 1. install the EAS CLI
npm install --global eas-cli

# 2. Build APK preview file
npx eas build -p android --profile preview

# or build a production ready Android App Bundle
npx eas build --p android --release-channel release --profile production
```

```js
// EAS JSON config
{
  "cli": {
    "version": "YOUR EAS CLI VERSION"
  },
  "build": {
    "development": {
      // ...
      "ios": {
        // ...
      }
    },
    "preview": {
      "android": {
        "buildType": "apk"
      },
      "ios": {
        // ...
      }
    },
    "release": {
      "releaseChannel": "release"
    },
    "production": {
      "ios": {
        // ...
      }
    }
  },
  "submit": {
    "production": {}
  }
}




[Amschel](https://github.com/amschel99)
