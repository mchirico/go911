

## go911

This puts data into BigQuery

```
docker run --rm -it aipiggybot/activeinc

# For non daemon
docker  run --rm -it --name activinc -a stdout -a stderr  aipiggybot/activeinc > activInc

docker  run --rm -it --name activinc  -d  aipiggybot/activeinc
docker logs  activinc

docker attach activinc

# To detach the tty without exiting the shell,
# use the escape sequence Ctrl-p + Ctrl-q


```


## Don't forget golint

```

golint -set_exit_status $(go list ./... | grep -v /vendor/)

```


