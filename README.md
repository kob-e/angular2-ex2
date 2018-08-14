# Angular 2 create and delpoy for first time

First time creating and deploying angular2 app

## Getting Started

These instructions teach you how to create and deploy angular2 using Firebase and Angular2 CLI

### Prerequisites

What things you need to install the software and how to install them

- nodejs
- npm
- git
- angular2 CLI

### IDE
VS code [https://code.visualstudio.com/]

### Installing

A step by step 

nodejs & npm:
```
[https://nodejs.org/en/download/]
```

git:
```
[https://git-scm.com/book/en/v2/Getting-Started-Installing-Git]
```

angular2 CLI:
```
$ npm install angular-cli -g
```


## Create your app

Create app: 
```$ ng new my-app```

Enter app directory: 
```$ cd my-app```

Run app: 
```$ ng serve```


goto [http://localhost:4200] and see if app works.

## Deployment
build app for deploy:
```$ ng build --prod```

goto [https://console.firebase.google.com/] and create a new Firebase project.

install firebase tools:
 ```$ npm install -g firebase-tools```

deploy to firebase:
```$ firebase login```

after authentication, run:
```$ firebase init```

First of all you're being asked which of the Firebase client features you want to use. Select the option Hosting: Configure and deploy Firebase Hosting site. Next the Firebase client will ask which folder to use for deployment. Type in dist. That is important because that is the location where our production build is stored. 
 
Next the question is ask if this app is a single page app and if it should rewrite all URLs to index.html. In our case we need to answer yes. 
 
Last question is if Firebase should over write file index.html. The answer to that question is no.


now run:
 ```$ firebase deploy```

## References

* **Hosting Angular 2 Applications On Firebase** - *Initial work* - [Sebastian Eschweiler](https://medium.com/codingthesmartway-com-blog/hosting-angular-2-applications-on-firebase-f194688c978d#.gt2pkhomp)

# Your submission
Should include the link of your firebase url with the app in README.md file and github should have project files.


#Submission date:

Sumbission rules:

all files should be in the github assignment repository.
you should include a link to Firebase url in README.md file.

# angular2-ex2
second exercise - using components

---

## exercise 1 summary:
### Create angular2 app:
> we use `my-app` as example for an application name
`$ ng new my-app`

`$ cd my-app`

`$ ng serve`

goto [http://localhost:4200](http://localhost:4200) and see if app works.

### Deployment

`$ npm install -g firebase-tools`

`$ firebase login`

`$ firebase init`
> use dist folder as public

`$ ng build --prod`

`$ firebase deploy`

## Creating new components:
> we use `cmpnt-name` as example for a component name

use the command `ng generate component cmpnt-name`
> you can use the the short command `ng g c cmpnt-name`

---
# What to do?
Create a new app (don't use the app from exercise 1).
Create a new component for app navigation menu. call the component `nav-menu`.
now create a new component again called `nav-item`.
nav menu should include an array of 4 objects, each object represent an item in the navigation menu. (think which properties it should have). the navigation menu template should iterate on the array and make the navigation items, pass the object to `nav-item` with `@Input()` decorator.
Style the app as you wish.

##
how to import js libraries

search for typings: https://microsoft.github.io/TypeSearch/
