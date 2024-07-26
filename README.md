## Features
- JWT authentication
- Create, update, and delete posts and comments
- Upvote/downvote posts and comments
- Nested comments threading
- Home page feed (front page)
- Subreddit specific feed
- Create subreddits
- Light and dark mode

## Installation
1. Clone this repository

```
git clone https://github.com/zorogotty14/subreddit-clone-react.git
cd subreddit-clone-react
```

2. Install backend dependencies

```
cd subreddit-clone-react-backend
npm install
```

3. Install frontend dependencies

```
cd subreddit-clone-react-frontend
npm install
```

4. Create config folder in the backend

```
cd subreddit-clone-react-backend
mkdir config
```

5. Configure environment variables. Create a `dev.env` file in the config folder, and paste the following (filling in your own postgres password and JWT secret)
```
PORT=5000
PG_HOST=localhost
PG_PORT=5432
PG_DBNAME=reddit-clone
PG_USER=postgres
PG_PASSWORD=<YOUR_PASSWORD>
JWT_SECRET=<YOUR_SECRET>

```

6. Create a postgres database named 'reddit-clone'

7. Run the database migrations

```
cd subreddit-clone-react-backend
npm run db-migrate up
```

## Usage
1. Start server

```
cd subreddit-clone-react-backend
npm run dev
```

2. Start client
```
cd subreddit-clone-react-frontend
npm start
```