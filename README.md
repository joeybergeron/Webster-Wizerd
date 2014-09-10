Using the Merriam - Webster API, which happens to be XML, and converting it into JSON data so that it can be useable through backbonejs & lodash templating. 


# How to use your server
1. clone / copy the files (server.js, package.json, Procfile) to your computer or project folder
2. `npm init`
3. `npm install`
4. `echo "node_modules" > .gitignore`
5. `node server.js <port number>` - where port number is any number (try 9000 for starters)
6. open your browser to `localhost:<port number>`
7. When you are ready to turn off the server, hit `CTRL + C`

# What does this give you?
1. Myth CSS PostProcessor (http://myth.io)
2. serves you files all nice and dandy
3. sets us up to push our own servers to heroku! (more to come)

# Want to push your local server to a live server?
1. setup a Heroku account
2. install the Heroku toolbelt: https://s3.amazonaws.com/assets.heroku.com/heroku-toolbelt/heroku-toolbelt.pkg
3. run `heroku login` in your terminal
4. create a random Heroku server with `heroku create`; this will register a remote git endpoint for you (`git remote -v`), which should now show Github (origin) and Heroku
5. then finally push your code repo up to Heroku (yes you can push to Github OR Heroku!) via a git push: `git push heroku master`
6. run `heroku ps:scale web=1` to spin-up some resources for your app
7. from here on out, anytime you want to push to the same heroku server, you only need to repeat step 6.
