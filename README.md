# laradock-cli
A small commandline tool to create, start, stop laradock, or enter the workspace

# Install

`composer global require lorinlee/laradock-cli`

# Usage
```
# Enter the laravel project directory

# Create laradock
laradock init

# Start containers
laradock up nginx mysql redis

# Stop containers
laradock stop nginx 
# Or stop all containers
laradock stop

# Enter workspace
laradock bash
# Or use root
laradock bash --root

# List all containers
laradock ps

# Edit docker-compose.yml
laradock config
```

Now you can use your own repo

```
# Set repo config
laradock repo myownrepo git@github.com:lorinlee/laradock.git

# Set default repo
laradock repo config_default myownrepo

# Prefer to use submodules (default no)
laradock repo config_submodule yes

# Disable enable the use of the default containers (default yes)
laradock repo config_use_default_container yes

# Use configured repo to init
laradock init myownrepo
```

# License
Apache License
