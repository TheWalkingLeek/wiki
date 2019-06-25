## What does it do?

Simple Auth is an ember addon meant to be used for authentication regardless of your application structure.

* It maintains the clientside session
* It authenticates the user to your backend server or other providers (Facebook, Google, ...)
* It authorizes requests

## How does it work?

Ember Simple Auth consists of 4 main building blocks - the session, a session store, authenticators and (optionally) authorizers.

* The session service provides methods for authenticating and invalidating the session.
* The session store persists the session state so that it survives a page reload. It also synchronizes the session state across multiple tabs or windows of the application
* Authenticators authenticate the session using multiple authentication services such as Facebook, Google or Github
* Authorizers use the data retrieved by an authenticator and stored in the session to generate authorization data that can be injected into outgoing requests such as Ember Data requests.

https://github.com/simplabs/ember-simple-auth