# Orchestration

Using docker-compose and in the future k8s to spin up our containers. 

Currently includes

- soba_web
- soba_api
- architecture
- engineering_blog

### On start

See https://git-scm.com/book/en/v2/Git-Tools-Submodules

First clone:

```
git clone --recurse-submodules git@github.com:socraticbananas/orchestration.git
```

If you forget the `--recurse-submodules` run

```
git clone git@github.com:socraticbananas/orchestration.git
git submodule update --init --recursive
```

### Refreshing submodules

Update all modules from `master`

```
git submodule update --remote
```

Or, if you are only interested in one, updating a specific submodule
```
cd repo/
git fetch
git merge origin/master
```

### Fetching changes to orchestration repo + updates to submodules

```
git pull
git submodule update --init --recursive
```

## Todo

Read the submodule docs. Add k8s.