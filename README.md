# README
For this to run you need to delete `config/credentials.yml.enc`,  run `rake secret` keep note of the secret and add it to rails credentials like this `EDITOR=nano rails credentials:edit` and add the following code 
```
devise:
  jwt_secret_key: <rake secret key>
```

`ctrl+x -> y -> enter`

Now create a new `.env` file `touch .env` on the top level of the app, and add `DEVISE_JWT_SECRET_KEY=<rake secret key>`.
`rails db:create` `rails db:migrate` `rails s` to run the app with JWT auth enabled.
