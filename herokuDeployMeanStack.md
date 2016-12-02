#Deploy MEAN Stack on Heroku

1. Update package.json file to include `"start": "node index.js"`
```
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "start": "node index.js"
},
```
2. Ensure git repository is fully committed

3. Login to heroku `heroku login`

4. Create heroku remote `heroku git:remote -a APPNAME`

5. Verify heroku remote `git remote -v`

##Adding mongod to heroku

1. Run `heroku addons:create mongolab`

 * Add credit card information in heroku if not already updated

2. Verify heroku configuration: `heroku config`

  * Should see: `MONGODB_URI: mongodb://heroku_xxxxxxxx`

3. Configure database connection in your connection.js

`mongoose.connect(process.env.MONGODB_URI || "mongodb://localhost/YOURDATABASENAME")`

4. Push changes to heroku `git push heroku master`

5. Seed your database `heroku run node db/seed.js`

6. Open your application `heroku open`

  * For angular without location provider Add /#/ to the end of the heroku url

  * In the event of err, check heroku log `heroku logs -t`
