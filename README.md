# vue-social-login

A basic social login PWA project example using **Vue**, **Firebase** and **Bulma**.

## Created as
```bash
Vue CLI v3.11.0
? Please pick a preset: Manually select features
? Check the features needed for your project: Babel, PWA, Router, CSS Pre-processors, Linter
? Use history mode for router? (Requires proper server setup for index fallback in production) Yes
? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Sass/SCSS (with dart-sass)
? Pick a linter / formatter config: Basic
? Pick additional lint features: (Press <space> to select, <a> to toggle all, <i> to invert selection)Lint on save
? Where do you prefer placing config for Babel, PostCSS, ESLint, etc.? In dedicated config files
```

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn run serve
```

### Compiles and minifies for production
```
yarn run build
```

### Run your tests
```
yarn run test
```

### Lints and fixes files
```
yarn run lint
```

### Firebase Deploy

To connect your local machine to your Firebase account
```bash
firebase login
```

To build and deploys the dist folder content to your Firebase project
```bash
npm run build && firebase deploy
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### Libraries
[Bulma Social](https://github.com/aldi/bulma-social)

### References
[PWA: Home Screan + Push Notification](https://medium.com/@n11sh1/how-to-build-pwa-w-vue-cli-3-service-workers-add-to-home-screen-push-notifications-b519c49e142d)

[Full guide to using Font Awesome icons in Vue.js apps](https://blog.logrocket.com/full-guide-to-using-font-awesome-icons-in-vue-js-apps-5574c74d9b2d/)