# remote mode
Experimental feature.  
`export TASK_X_REMOTE_TASKFILES=1` check .env file.  

Whenever you run a remote Taskfile, the latest copy will be downloaded from the internet and cached locally (.task/remote).

```bash
task golden-sample:hello

# no security prompt
task golden-sample:hello --yes

# use only local cached version
task golden-sample:hello --offline

# force download without running any task
task --download

# default timout is 10s but can be increased with --timeout 30s
```

