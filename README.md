#Submission date:
14/03/2017

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