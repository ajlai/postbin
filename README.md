postbin
=======

Postbin written in Sinatra

### Instructions for self-hosting on Heroku
#### 1\. Clone it
```bash
$ git clone https://github.com/ajlai/postbin.git
```
#### 2\. Create the app on Heroku
```bash
$ cd postbin
$ heroku create my-very-own-postbin
```
#### 3\. Setup the database (the `_COLOR_URL` part may be different on your installation)
```bash
$ heroku addons:add heroku-postgresql
...
Attached as HEROKU_POSTGRESQL_BLACK_URL
...
$ heroku pg:promote HEROKU_POSTGRESQL_BLACK_URL
Promoting HEROKU_POSTGRESQL_BLACK_URL to DATABASE_URL... done
```
#### 4\. Launch it!
```bash
$ git push heroku master
...
...
...
       http://my-very-own-postbin.herokuapp.com deployed to Heroku
```
