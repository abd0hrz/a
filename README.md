# Inventory management mern Stack application with mongoDB, Express, React and NodeJS


## Features
- API endpoints with Express
- Authentication with JSON Web Token including User Registration, Login and Password Reset
- CRUD functionality on various routes(auth, users, allUsers, purchases, products, customers, suppliers, sales). I'll probably add more later
- Users can update their account info(yet to implement email verification but that would be later)
- Upload image with multer and save to Cloudinary
- Protect routes to only be accessed by logged-in users
- Frontend pages with React and SCSS
- Routing with React Router V6
- CRUD functionality
- Implement pagination on the front-end
- Connect frontend to backend using Axios
- Manage state with Redux Toolkit
- Dashboard for product management
- Utilize "express-async-handler" package
- Error handling in Express
- Hash passwords
- User profile page
- Contact us page

<!-- Add other features -->

## Usage

- `npm install`

- Go to the `sample.env` file and follow the instructions there. Run `npm run server` to start the Express API, run `npm run client` to run the React Frontend and `npm run dev` to run both of them concurrently.

## Todo

- Frontend Responsiveness: I used just styled components. So, I'll make out time to ensure the app is fully responsive soon.
  >update: done

- Display weekly and monthly Sales and purchases on the dashboard along with total profit made during the period.

- Search

- Users should be able to edit their details(change password, name, email, username, company): There's already endpoints for this on the BE but they've not been implemented on the FE

- Remove some lorem ipsums that are still on the landing page.

- Deploy to Heroku or Zeit Now
  >update: done

## API docs

### Routes

- `/api/allUsers`: This GET route serves json of all registers users as an array of objects(when parsed). Fields include `memberSince`, `username`, `email`, `company`

- `/api/auth`: This route does two things. The GET method authenticates a logged in user(private route and requires a token) by using the token to check for the user. Thereby returning the currently logged in user. The POST method is used for logging in a user and authenticating them. Fields required: one of of `email` or `username` and `password`.

- `/api/customers`: This has GET, POST, PUT and DEL methods. They perform CRUD functionalities for an authenticated user's customers.

- `/api/products`: This has GET, POST, PUT and DEL methods. They perform CRUD functionalities for an authenticated user's products.

- `/api/purchases`: This has GET, POST, PUT and DEL methods. They perform CRUD functionalities for an authenticated user's purchases.

- `/api/sales`: This has GET, POST, PUT and DEL methods. They perform CRUD functionalities for an authenticated user's sales.

- `/api/suppliers`: This has GET, POST, PUT and DEL methods. They perform CRUD functionalities for an authenticated user's suppliers.

- `/api/users`: This has POST, PUT and DEL methods. They respectively create users, edit users' details and delete users.

-----------------

