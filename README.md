#Sparted backend V2

Custom app name :

```export APP="sparted"```

App creation:

```docker run -it --rm -v $PWD:/src kallikrein/sails sails new $APP```

Set ownership of the app folder

```sudo chown -R $USER $APP```

App lift :

```docker-compose up```

Useful aliases

```alias drun='docker run -it --rm'```

```alias sails='drun -v $PWD:/src kallikrein/sails-tools sails'```

Sails automated generation :

(*NB: these features are extensively covered by the Waterlock module, designing JWT auth for sails*)
https://github.com/waterlock/waterlock
http://waterlock.ninja
The stability and efficiency of this module should be tested.


- api/controller/AuthController.js
```
sails generate controller Auth
```
- api/models/Users.js
```
sails generate model Users
```
- api/policies/hasJsonWebToken.js
```
sails generate policy hasJsonWebToken
```
