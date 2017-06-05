# Express server with Passport and OAuth

This demonstrates a fairly minimal third-party OAuth (including API auth using JWT and HTTP-only cookies).


## Install

```shell
git clone https://github.com/dev-academy-challenges/passport-oauth-demo.git
cd passport-oauth-demo
npm install
```


## Setup

* Go to https://dev.twitter.com and create a new app

```shell
mv .env.example .env
```

* Edit `.env` to include your Twitter app's keys


## Start/debug

```shell
npm start
# or npm run debug
```

You should be able to use Postman to go to [http://localhost:3000/api/v1/open](http://localhost:3000/api/v1/open) because that endpoint isn't protected. However, [http://localhost:3000/api/v1/closed](http://localhost:3000/api/v1/closed) is protected, so you shouldn't be able to access it.

* Using your browser, go to [http://localhost:3000/api/v1/auth/twitter](http://localhost:3000/api/v1/auth/twitter) and authorise the application.
* Using Postman, go to [http://localhost:3000](http://localhost:3000) to verify a token was issued.
* Using Postman, go to [http://localhost:3000/api/v1/closed](http://localhost:3000/api/v1/closed) to ensure you have access.


## Next

Build out the rest of this app experience :wink:
