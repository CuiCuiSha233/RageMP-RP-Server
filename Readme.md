# RageMP Dev

## Running Server
Windows
``` bash
npm i -g pm2 # install pm2 

cd /your/ragemp/server-files

pm2 start server.exe --watch # starts the server.exe in watch mode. it will restart on any file changes inside the server-files folder
  
pm2 stop server --watch # its important to stop it with the --watch flag otherwise it will still restart.

pm2 logs server # will show you the logs
```

Linux
``` bash
nodemon --watch packages --watch client_packages --exec \"./server.exe\"
```