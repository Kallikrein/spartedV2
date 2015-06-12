#Sparted backend V2

Custom app name :

```export APP="sparted"```

App creation:

```docker run -it --rm -v $PWD:/src kallikrein/sails sails new $APP```

Set ownership of the app folder

```sudo chown -R $USER $APP```

App lift :

```docker-compoe up```
