<img src="https://single-spa.js.org/img/logo-white-bgblue.svg" width="50" height="50">

[![npm version](https://img.shields.io/npm/v/single-spa-root.svg?style=flat-square)](https://www.npmjs.org/package/single-spa-root)

# single-spa-root

Single-spa application example which imports registered applications from NPM packages and manages authentication features as login.

The login validation is harcoded in code and the credentials are:

| User          | Password      |     
| ------------- |:-------------:|
| admin         | 12345         |

## 💻 Run in localhost

If you prefer run this application in localhost you must follow next steps:

```
npm install
```

```
npm run serve
```

Finally you only have to open [http://localhost:8080](http://localhost:8080) in a browser to see the app running


## single-spa applications

This application is a root-application that inits a single-spa application that integrates several registered applications:

- [single-spa-login](https://github.com/Will-wpl/single-spa-login)
- [single-spa-layout](https://github.com/Will-wpl/single-spa-layout)
- [single-spa-home-app-new](https://github.com/Will-wpl/single-spa-home-app-new)
- [single-spa-angular](https://github.com/Will-wpl/single-spa-angular)
- [single-spa-vue](https://github.com/Will-wpl/single-spa-vue)
- [single-spa-react](https://github.com/Will-wpl/single-spa-react)

### <img src="https://vuejs.org/images/logo.png" width="25" height="25"> single-spa-auth-app

This application is displayed by default as there is no logged in user. A login form is printed and the credentials can be set for perform the login and access to the private views.

### <img src="https://vuejs.org/images/logo.png" width="25" height="25"> single-spa-layout-app

This application contains **header**, **navbar** and **footer** sections, **navigation** between registered applications and **/login** redirection if **logout** link is clicked or **token** is removed from **sessionStorage**.

### <img src="https://angularjs.org/img/ng-logo.png" width="25" height="25"> single-spa-home-app

This application is developed with **Angular JS** and is mounted when home icon in navbar is clicked. In that case the url will be **/** and all **Angular JS** routes will be managed by **angular-ui-router**. By the moment this application has only one default routed view.

### <img src="https://angular.io/assets/images/logos/angular/angular.png" width="25" height="25"> single-spa-angular-app

This application is developed with **Angular v8** and is mounted when **Angular** navbar item is clicked. In that case the url will be **/angular** and all **Angular** routes will be managed by **angular router**.

### <img src="https://vuejs.org/images/logo.png" width="25" height="25"> single-spa-vue-app

This application is developed with **Vue** and is mounted when **Vue** navbar item is clicked. In that case the url will be **/vue** and all **Vue** routes will be managed by **vue-router**.

### <img src="https://cdn.auth0.com/blog/react-js/react.png" width="25" height="25"> single-spa-react-app

This application is developed with **React** and is mounted when **React** navbar item is clicked. In that case the url will be **/react** and all **React** routes will be managed by **react-router-dom**.

