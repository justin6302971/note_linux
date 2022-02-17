``` bash
# list all the process listen on the port
lsof -i:{port}    

# kill all the process listen on the port
kill -9 $(lsof -t -i:{port})

```