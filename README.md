Junon.io
=======
Junon.io is a co-op multiplayer survival game where your goal is to build your own space-station, grow your colony, and defend it against hostile threats.

Installation (linux)
--------
1. Install Node.js 16.15.0 (ideally using [nvm](https://github.com/nvm-sh/nvm) )
2. Install MySQL
3. Install project dependencies
```
   cd ~/junon
   npm install
```

4. Setup database using the command below. It is assumed that your mysql user is 'root' with empty password. To override this, define `JUNON_DB_USER` and `JUNON_DB_PASS` in a .env file, or in the /packages/junon-common/db/config.js file.
```
        npm run db:setup
```

Running
--------
1. Environment
You need to choose environment(development by default):
- development: recommended for testing stuff
- staging: pre-production environment. Almost identical
- production: full application
```
    export NODE_ENV=staging
```
If using staging or production you should define `IP_ADDRESS` too:
```
    export IP_ADDRESS="server's ip"
```

2. Run client
```
    npm run client
```

3. Run server
```
    npm run server
    Go to http://localhost:8001 to access Junon io homepage
```

4. Debugging
---------
```
    Enter "chrome://inspect/" in chrome browser
    Click "Open dedicated DevTools for Node"
```


Contributing guide
---------

  See https://www.youtube.com/channel/UCMuok-F6ElORq7aKyyFDgqw for tutorials related to running/contributing
