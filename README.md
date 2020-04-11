


[![Build Status](https://travis-ci.org/mchirico/activeIncident.svg?branch=master)](https://travis-ci.org/mchirico/activeIncident)
[![codecov](https://codecov.io/gh/mchirico/activeIncident/branch/master/graph/badge.svg)](https://codecov.io/gh/mchirico/activeIncident)
[![Build Status](https://mchirico.visualstudio.com/activeIncident/_apis/build/status/mchirico.activeIncident?branchName=master)](https://mchirico.visualstudio.com/activeIncident/_build/latest?definitionId=7&branchName=master)
[![Board Status](https://mchirico.visualstudio.com/f2f93792-8538-42e3-99ee-11cff3492aa9/876f6067-eebb-428e-a0a4-0fdaa6e6889b/_apis/work/boardbadge/745b312c-827d-41ed-99d6-b0ad733b51b7)](https://mchirico.visualstudio.com/f2f93792-8538-42e3-99ee-11cff3492aa9/_boards/board/t/876f6067-eebb-428e-a0a4-0fdaa6e6889b/Microsoft.RequirementCategory/)

# activeIncident

## Docker
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


