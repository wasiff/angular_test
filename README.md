# AngularTest

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.2.1.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Test Details

#### Application Setup 
Clone the application and run `npm intall` to install the required npm libraries. There are 3 routes created under the application `/login` `/register` `/profile`, we do not expect you to write/update any html/css in the application

#### Tasks are as follows:

- Create register component form using Reactive Forms in Angular
- Create validations for the form, make all fields required, make password min 5 and max 12 characters long and confirm password validation.
- Create login component form using Reactive Forms in Angular
- Create validations for the form, make all fields required and make password min 5 and max 12 characters long.
- Login user and save authentication details in Local Storage
- Create a service to call the APIs (API Details below)
- In profile component call the `/profile` api and display user profile details (do not use the data from local storage)
- Create an Authentication Guard and protect the route `/profile` so only logged in user can access the route
- Create an Http Interceptor and make sure the Bearer token in passed in header if the user is logged in

##### GOOD LUCK!



## API Details

### Login:
URL: `https://infinite-crag-97613.herokuapp.com/auth/login`  

Type: `POST`
#### payload:
```js
{
    "email": string,
    "password": string
}
```

### Register:
URL: `https://infinite-crag-97613.herokuapp.com/auth/register`  

Type: `POST`
#### payload:
```js
{
    "fullname": string,
    "email": string,
    "password": string
}
```

### Profile:
URL: `https://infinite-crag-97613.herokuapp.com/auth/profile`  

Type: `GET`
#### payload:
```js
None
```
#### Header:
`Authorization: Bearer <token>`

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.
