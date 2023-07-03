# README
For this to run you need to run `rake secret` keep note of the secret and add it to rails credentials liike this `EDITOR=nano rails credentials:edit` and add the following code 
```
devise:
  jwt_secret_key: <rake secret key>
```

`ctrl+x -> y -> enter`
