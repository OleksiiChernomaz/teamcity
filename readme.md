# Dockerized Teamcity with 1 agent

- quick start if you just want to try the tool, or want to use it on a regular base 
- original TeamCity package: nothing removed or changed, just a skeleton for your application within `docker-compose.yml` file

# What is Teamcity
 
 Quite powerful tool to create CI/CD pipelines. Professional version (free of charge) has limitations in amount of builds and connected agents. But usually it's more then enough for small projects.
 
 Read more on the official site: https://www.jetbrains.com/teamcity/   


# How to use

- clone or fork project, copy-pasting might work as well :D
- Configure a little bit, copy example `env.dist` file and adjust it:
```bash
cp ./env.dist ./.env
```
- run stack using docker-compose (as an example, you can take a look at the `./docker-compose.yml``):
```bash
docker-compose up
```
- files, which must be persisted, are in `./data` folder
- logs are stored in `./logs` folder.
`
# How to contribute

> ### Note 
> 
> This container was created for internal purposes and meets all the requirements to 
> start use `TeamCity` quickly.

- checkout appropriate branch
- make sure that you have pulled all the latest changes from the remote branch
- make all the changes, create a pull request
- after PR is merged, your changes would be applied during next release

# Known bugs

- you tell :)

# To make a test build on your local machine:

```
docker-compose build
```

