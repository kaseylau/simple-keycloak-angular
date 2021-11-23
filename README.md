# Simple Keycloak Angular

Simple angular app for SSO with local keycloak


# Before running the application

In Keycloak,
- Run keycloak server
- Create realm `Test` (Case sensitive)
- Create Client `frontend-app`
- Configure the Client as public client with standard flow only. Add `http://localhost:4200/*` to the Valid Redirect URLs and a '`+`' to Web Origin.

In this app,
- Go to `app.module.ts` to edit the keycloak init config (url, realm, clientId)
- Go to `app.component.ts` to edit the login scope

# Running the application

Once the Keycloak server is up and running you can start the client application by running `ng serve` (or `npm start`) and navigating to `http://localhost:4200/` just like any other Angular CLI application.