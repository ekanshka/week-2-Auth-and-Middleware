# Mini Project to practice authentication using jwt and more middlewares

## Tech Stack 🚀💻
### Backend -> TypeScript, Express, jwt
### Database -> MongoDB 
### Frontend -> React, Tailwind, Recoil (state manager)

#

## Tests Done (POSTMAN and FRONTEND): ✅ 👍
- working signup feature 
- working signin feature
    - store the access token from the request in the localStorage
    - use it in every pages request header

- authenticated user allowed on surf across protected pages (with and without persisted state)

- display current user's data on profile page/all pages
    - you can introduce recoil here to store the user's data globally

- make multiple new users and surf from their acc with their data

#

## Bugs : ❌
- none for the required functioning.
- ~very slight bug, navbar doesn't update after logout redirect to signin page~ - FIXED ✅
- ~navigating back to old pages from browser still show current user's details which goes away at hard refresh~ - FIXED ✅


#

## Things learnt : 🎊
- Provide a jwt token encoded with some user information (provided at signup or something) ✅
- Send the token back in every request header that needs the auth/login (use a middleware to authenticate) ✅

#

- Bring in mongodb, use that to actually store user data at signup and sign it in the jwt along with username ✅
- and when on signin, fetch user data from the id after decoding the jwt ✅

#

- Introduce React to test all the routes with a frontend ✅
- Send backend requests with axios ✅
- Implement the logic to store the access token in the localStorage and use it in subsequent requests ✅
- Display the user data recieved after login on the profile page (closing browser and no signin) ✅

- Use Recoil to manage user data after login and persists it using the help of recoil-persist library which makes it much easier to persist atom ✅

#

## Run : 🚀
- Run "npm install" in root folder
- Go into backend folder and make a new .env file and store the values for:
    - JWT_SECRET, MONGO_URL
- Run "npm run build" in root folder
- Run "npm run start" in root folder

