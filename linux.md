# linux commands
``` bash
# list by program
lsof -c {program}

# list all ports
lsof -i TCP -s TCP:ESTABLISHED

lsof -i TCP -s TCP:LISTEN

# list all the process listen on the port
lsof -i:{port}    

# kill all the process listen on the port
kill -9 $(lsof -t -i:{port})



```


## reference
1. [linux-lsof-command-list-tutorial-examples](https://blog.gtwang.org/linux/linux-lsof-command-list-open-files-tutorial-examples/)