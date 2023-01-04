# tutorial-dev-camper-api

1. npm i express dotenv - loads environment variables

   require('dotenv').config()

   Create a .env file in the root dir of your project. Add env specific variables on new lines in the form of NAME=VALUE. For example:

   ```
   DB_HOST=localhost
   DB_USER=root
   DB_PASS=s1mpl3
   ```
   
   process.env how has the keys and values you defined in your .env file.

   ```
    const db = require('db')
    db.connect({
        host: process.env.DB_HOST,
        username: process.env.DB_USER,
        password: process.env.DB_PASS,
    })
   ```

2. npm i -D nodemon

3. examples

   ```
   res.send("Hello World");
   res.json({name: Tommy});
   res.sendStatus(400);
   res.status(400).json({ success: false})
   res.status(200).json({success: true, data: { id: 1}});
   ```

4. mongodb.com - download mongodb compass pkg

5. mongoose - queries against database. npm i mongoose

6. 