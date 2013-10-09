## Environment Variables with Daniel
What does the ENV mean in the following line?!
```
  set :database, ENV['DATABASE_URL']
```

1. ENV variables are set on your computer.
1. ENV is a key-value pair store for data
1. From your terminal: `echo $PATH`
1. Sometimes you have secret stuff you don't want hard coded (config variables)
1. Set those using Environment variables:
1. On Heroku `heroku config:set NAME_OF_VARIABLE=AwesomeVariable
1. On local `export NAME_OF_VARIABLE=AwesomeVariable
1. Using `dotenv` 

in your `.env` file
```
AWESOME_VAR=Zee is awesome
```
require 'dotenv'
p ENV['AWESOME_VAR'] # Nil :(
Dotenv.load
p ENV['AWESOME_VAR'] # Zee is awesome
```

You may want to use .gitignore to ignore your .env file

```
.env
```
