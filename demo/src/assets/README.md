<p align="center">
  <img height="256px" width="256px" style="text-align: center;" src="https://cdn.rawgit.com/firebaseui/ng-bootstrap/master/demo/src/assets/logo.svg">
</p>

# @firebaseui/ng-bootstrap - Angular Bootstrap UI library for firebase authentication powered by @ng-bootstrap

[![npm version](https://badge.fury.io/js/%40firebaseui%2Fng-bootstrap.svg)](https://badge.fury.io/js/%40firebaseui%2Fng-bootstrap)
[![npm demo](https://img.shields.io/badge/demo-online-ed1c46.svg)](https://firebaseui.github.io/ng-bootstrap)
[![Join the chat at https://gitter.im/firebaseui/Lobby](https://badges.gitter.im/firebaseui/Lobby.svg)](https://gitter.im/firebaseui/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![CircleCI branch](https://img.shields.io/circleci/project/github/firebaseui/ng-bootstrap/master.svg?label=circleci)](https://circleci.com/gh/firebaseui/ng-bootstrap)
[![Coverage Status](https://coveralls.io/repos/github/firebaseui/ng-bootstrap/badge.svg?branch=master)](https://coveralls.io/github/firebaseui/ng-bootstrap?branch=master)
[![dependency Status](https://david-dm.org/firebaseui/ng-bootstrap/status.svg)](https://david-dm.org/firebaseui/ng-bootstrap)
[![devDependency Status](https://david-dm.org/firebaseui/ng-bootstrap/dev-status.svg?branch=master)](https://david-dm.org/firebaseui/ng-bootstrap#info=devDependencies)
[![Greenkeeper Badge](https://badges.greenkeeper.io/firebaseui/ng-bootstrap.svg)](https://greenkeeper.io/)
[![license](https://img.shields.io/github/license/firebaseui/ng-bootstrap.svg?style=flat-square)](https://github.com/firebaseui/ng-bootstrap/blob/master/LICENSE)

## Built by and for developers :heart:
Do you have any question or suggestion ? Please do not hesitate to contact us!
Alternatively, provide a PR | open an appropriate issue [here](https://github.com/firebaseui/ng-bootstrap/issues)

If did you like this project, support [@firebaseui/ng-bootstrap](https://github.com/firebaseui/ng-bootstrap) 
by starring :star: and sharing it :loudspeaker:

## Table of Contents
- [@firebaseui/ng-bootstrap :heart: ngx-auth-firebaseui | vs firebaseui-web](#vs)
- [Why to use @firebaseui/ng-bootstrap ?](#@firebaseui/ng-bootstrap)
- [Library's components](#components)
- [Supported Providers](#supported-procress-and-actions)
- [Supported Processes and Actions](#supported-procress-and-actions)
- [Requirements](#requirements)
- [Demo](#demo)
- [Features](#features)
- [Examples](#examples)
- [Documentation](#documentation)
- [Screenshots](#screenshots)
- [Peer Dependencies](#peerDependencies)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Additional Requirements - font awesome icons](#additional-requirements-fontawesome-icons)
- [Additional Requirements - assets](#additional-requirements-assets)
- [Run Demo App Locally](#run-demo-app-locally)
- [Development](#development)
- [Other Angular Libraries](#other-angular-libraries)
- [Support](#support)
- [License](#license)

<a name="vs"/>

## ngx-auth-firebaseui vs firebaseui-web

| Features                                                      | @firebaseui/ng-bootstrap    | ngx-auth-firebaseui       | firebaseui  |
| --------------------------------------------------------------|:-------------:              |:-------------:|           :-------------------:  |
| Sign Up                                                       | :heavy_check_mark:  | :heavy_check_mark:    |  :heavy_check_mark:    |
| Sign In                                                       | :heavy_check_mark:  | :heavy_check_mark:    |  :heavy_check_mark:    |
| Sign In Anonymously                                           | :heavy_check_mark:  | :heavy_check_mark:    |  :x:                   |
| Sign In with Google                                           | :soon:  | :heavy_check_mark:    |  :heavy_check_mark:    |
| Sign In with Facebook                                         | :soon:  | :heavy_check_mark:    |  :heavy_check_mark:    |
| Sign In with Twitter                                          | :soon:  | :heavy_check_mark:    |  :heavy_check_mark:    |
| Sign In with Github                                           | :soon:  | :heavy_check_mark:    |  :heavy_check_mark:    |
| Sign In with PhoneNumber                                      | :soon:  | :x:                   |  :heavy_check_mark:    |
| Sign out                                                      | :soon:  | :heavy_check_mark:    |  :x:                   |
| Sign in/up progress indicator                                 |  :heavy_check_mark: | :heavy_check_mark:    |  :x:                   |
| Password Strength indicator                                   | :soon: | :heavy_check_mark:    |  :x:                   |
| Forgot/Reset Password                                         | :heavy_check_mark:  | :heavy_check_mark:    |  :x:                   |
| Delete account                                                | :soon:  | :heavy_check_mark:    |  :x:                   |
| User Profile                                                  | :soon:  | :heavy_check_mark:    |  :x:                   |
| Check whether user's email is verified                        | :soon:  | :heavy_check_mark:    |  :x:                   |
| Edit user's display name (incl. validation)                   | :soon:  | :heavy_check_mark:    |  :x:                   |
| Edit user's email (incl. validation)                          | :soon:  | :heavy_check_mark:    |  :x:                   |
| Edit user's phone number (incl. validation)                   | :soon:  | :heavy_check_mark:    |  :x:                   |
| Configure your favorite auth provider in runtime              | :soon:  | :heavy_check_mark:    |  :x:                   |
| Sync user'auth with Firestore  [read more](FIRESTORE_SYNC.md) |  :heavy_check_mark: | :heavy_check_mark:    |  :x:                   |
| Angular v2-6 friendly                                         |  :heavy_check_mark:  | :heavy_check_mark:    |  :x:                   |
| Internationalization (i18n)                                   |  :soon: @angular v7  | :soon: @angular v7    |  :heavy_check_mark:    |
| Ionic/cordova support                                         |  :soon:  @firebaseui/ionic-auth   | :soon:  @firebaseui/ionic-auth |  :x:          |
| Real time form validation                                     |  :heavy_check_mark:   | :heavy_check_mark:    |  :x:                   |
| Easy to integrate                                             |  :heavy_check_mark:   | :heavy_check_mark:    |  :x:                   |
| Support Server Side Rendering                                 |  :heavy_check_mark:   | :heavy_check_mark:    |  :x:                   |
| Support SPA without further config                            |  :heavy_check_mark:  | :heavy_check_mark:    |  :x:                   |
| Support Safari private browsing                               |  :heavy_check_mark:   | :heavy_check_mark:    |  :x:                   |
| AWESOME                                                       |  :heavy_check_mark:   | :heavy_check_mark:    |  :interrobang:         |


<a name="why-to-use-ngx-auth-firebaseui"/>

## Why to use @firebaseui/ng-boostrap ?
- :gift_heart: it uses a responsive and accessible web design UX/UI from twitter bootstrap concepts and components (supporting desktop and mobile view).
- :lipstick: pick up your own theme! change the primary, secondary and danger colors whenever you need (e.g to support light and dark themes) via scss - bootstrap
- :ship: super easy to use with an angular based project (project that is created with the [angular-cli](https://cli.angular.io/))
- :soon: optional configuration
- :soon: configure your authentication providers in runtime
- :recycle: reusable components for every project that needs an authentication with a firebase project/app.
- :soon: built in feedback mechanism in form of a [alert](https://ng-bootstrap.github.io/#/components/alert/examples) when an error or any important event occurred.
- :soon: ability to sign out or even to delete totally the account
- :ghost: your client does not want to create an account in your project? Let him to sign in anonymously!
- :soon: user profile component to display user's data using <ngx-auth-firebaseui-user></ngx-auth-firebaseui-user> via `ngx-auth-firebaseui-user`
- :zap: update user profile as feature
- :fire: [Sync user's authentication with FIRESTORE](FIRESTORE_SYNC.md) **AUTOMATICALLY**
- :muscle: Forgot Password feature! Go and let your users to recover their passwords easily 
- :tada: Supports SSR - Server Side Rendering


<a name="components"/>

## Library's components
- `<ngb-auth-firebaseui>` used for the authentication process
-  :soon: `<ngb-auth-firebaseui-providers>` used to display only buttons for providers like googe, facebook, twitter and github
-  :soon: `<ngb-auth-firebaseui-user>` used to display/edit the data of the current authenticated user

<a name="supported-providers"/>

## Supported Providers:
- anonymously
- email and password (traditional)
- google :soon:
- facebook :soon:
- twitter :soon:
- github :soon:
- phone number :soon:

<a name="supported-procress-and-actions"/>

## Supported Processes and Actions:
- sign up
- sign in
- sign in Anonymously | with google, facebook, twitter, github
- sign out
- validation of password's strength while creating a new account using [ngx-material-password-strength](https://github.com/AnthonyNahas/ngx-material-password-strength) :soon:
- forgot/reset password
- sending email verifications
- delete user's account :soon:
- edit user's profile like email, name, (profile picture :soon:) and phone number :soon:
- firestore auto sync :fire:

<a name="requirements"/>

### Requirements:
- [ng-bootstrap - v2](https://www.npmjs.com/package/@ng-bootstrap/ng-bootstrap) 
- [angular forms - v6.x](https://www.npmjs.com/package/@angular/forms)
- [@angular/fire - v5.0.0-rc.11](https://www.npmjs.com/package/@angular/fire)
- [firebase - v5.x](https://www.npmjs.com/package/firebase)
- [font-awesome - v4.x](https://www.npmjs.com/package/font-awesome)

<a name="demo"/>

##  [Demo](https://ngx-auth-firebaseui.firebaseapp.com/)

- Try it out
```js
if(issues || feedback || you_need_more_features){
    // send me an email -> to: anthony.na@hotmail.de
}
```

## Dependencies
* [Angular](https://angular.io) (*requires* Angular 2 or higher, tested with v5 and v6)

## Installation
Install above dependencies via *npm*. 

Now install `@firebaseui/ng-bootstrap` via:
```shell
npm install --save @firebaseui/ng-bootstrap
```

---
##### SystemJS
>**Note**:If you are using `SystemJS`, you should adjust your configuration to point to the UMD bundle.
In your systemjs config file, `map` needs to tell the System loader where to look for `@firebaseui/ng-bootstrap`:
```js
map: {
  '@firebaseui/ng-bootstrap': 'node_modules/@firebaseui/ng-bootstrap/bundles/@firebaseui/ng-bootstrap.umd.js',
}
```
---

Once installed you need to import the main module:
```js
import { NgbAuthFirebaseUIModule } from '@firebaseui/ng-bootstrap';
```
The only remaining part is to list the imported module in your application module. The exact method will be slightly
different for the root (top-level) module for which you should end up with the code similar to (notice ` NgbAuthFirebaseUIModule.forRoot()`):
```js
import { NgbAuthFirebaseUIModule } from '@firebaseui/ng-bootstrap';

@NgModule({
  declarations: [AppComponent, ...],
  imports: [NgbAuthFirebaseUIModule.forRoot(), ...],  
  bootstrap: [AppComponent]
})
export class AppModule {
}
```

Other modules in your application can simply import ` NgbAuthFirebaseUIModule `:

```js
import { NgbAuthFirebaseUIModule } from '@firebaseui/ng-bootstrap';

@NgModule({
  declarations: [OtherComponent, ...],
  imports: [NgbAuthFirebaseUIModule, ...], 
})
export class OtherModule {
}
```

## Usage


<a name="run-demo-app-locally"/>

## Run Demo App Locally

- [clone this repo](https://github.com/firebaseui/ng-bootstrap.git) by running
```bash
$ git clone https://github.com/firebaseui/ng-bootstrap.git
```
- link the ngx-auth-firebaseui package
use gulp globally
```bash
$ gulp link
```
- navigate to the demo app directory
```bash
$ cd demo
```

- install the dependencies
```bash
$ npm i
```
- run/start/serve the app
```bash
$ npm run start
```
or
```bash
$ ng serve --open
```
- the app is now hosted by `http://localhost:4200/`

---

<a name="development"/>

## Development

To generate all `*.js`, `*.d.ts` and `*.metadata.json` files:

```bash
$ npm run build
```

To lint all `*.ts` files:

```bash
$ npm run lint
```
---


<a name="other-angular-libraries"/>

## Other Angular Libraries
- [ngx-material-pages](https://github.com/AnthonyNahas/ngx-material-pages)
- [@angular-material-extensions/password-strength](https://github.com/angular-material-extensions/password-strength)
- [@angular-material-extensions/pages](https://github.com/angular-material-extensions/pages)
- [@angular-material-extensions/contacts](https://github.com/angular-material-extensions/contacts)
- [@angular-material-extensions/faq](https://github.com/angular-material-extensions/faq)
- [@angular-material-extensions/jumbotron](https://github.com/angular-material-extensions/jumbotron)
- [@angular-material-extensions/google-maps-autocomplete](https://github.com/angular-material-extensions/google-maps-autocomplete)
- [@angular-material-extensions/combination-generator](https://github.com/angular-material-extensions/combination-generator)

---

## Support
+ Drop an email to: [Anthony Nahas](mailto:anthony.na@hotmail.de)
+ or open an appropriate [issue](https://github.com/firebaseui/ng-bootstrap/issues)
+ let us chat on [Gitter](https://gitter.im/ngx-auth-firebaseui/Lobby)
 
 Built by and for developers :heart: we will help you :punch:

---

<a name="license"/>

## License

Copyright (c) 2018 [Anthony Nahas](https://github.com/AnthonyNahas). Licensed under the MIT License (MIT)
