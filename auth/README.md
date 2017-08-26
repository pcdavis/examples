# Users, sessions and auth

This ReactQL project demonstrates one possible way you might implement user/password authorisation.

This is the first version; it will be expanded soon to add social logins.

## Features

* User sign-up form, with field validation (email validation via [isemail](https://www.npmjs.com/package/isemail))
* In-memory SQLite DB with `users` and `sessions` tables, running via [Sequelize v4](http://docs.sequelizejs.com/)
* Server-side sessions. Deleting the DB entry remotely kills the session
* Password hashing via [bcrypt](https://www.npmjs.com/package/bcrypt)
* GraphQL types representing users, sessions, [JWT tokens](https://www.npmjs.com/package/jsonwebtoken), field errors
* [Semantic UI React](https://react.semantic-ui.com) components and styling
* JWT tokens -- stored in both `localStorage` and via cookies, for subsequent SSR requests to render authenticated content on the server side, and for stateless environments such as mobile
* No modifications to the kit -- pure userland code

## Kit version

Based on ReactQL kit [v2.5.3](https://github.com/reactql/kit/releases/tag/2.5.3)