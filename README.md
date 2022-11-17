## MVP

The project is intended to allow users to learn about The Killers, listen to brief snippets of their music, and enjoy full playthroughs of covers I have personally created of some of their music. 

It includes typical navigation features such as dropdowns and navbars. It uses [React Router](https://reactrouter.com/docs/en/v6). It also has a fully functional admin section with authentication manually implemented (using Bcrypt for password hashing and manual database seeding with a key for verification of successful login state on the backend). Use the public username and password of "admin" to view the admin dashboard without being granted write access to the database.

The admin section allows for CRUD operations on the database to allow the addition of music to the public facing 'music-player' and 'covers' sections without the need to write additional code. Login to the admin dashboard persists until the 'LOGOUT' link is clicked in the dashboard nav, or until the page is manually refreshed/loaded in a new tab or window. If an admin bookmarks a page in the admin dashboard, they will be redirected to the login screen which, upon successful authentication, will redirect them back to the page they originally intended to visit.

Styles are highly customized, making use of tailwind to quickly prototype the UI as well as custom designed resources I made myself in Figma.

Additionally, custom hooks are used for managing authentication with react router and for updating the document title dynamically.

To visit the admin page, use the /build/admin endpoint. You may view, but not update database information using the login/password "admin" "admin".
