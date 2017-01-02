# kuzzle-plugin-template

This repository contains the boilerplate code you need to create a new plugin for Kuzzle 1.0.0-RC8 and above.

## Start developing a new plugin for Kuzzle

Fork this repository and name it as you like (e.g. `my-awesome-plugin`),
then clone your fork in a local directory.
In your local repository, rename all the occurrences of `kuzzle-plugin-template` in the following files

- `package.json`
- `dev/docker-compose.yml`
- `dev/pm2.json`

Then start the Kuzzle stack via docker-compose

```bash
$ docker-compose -f dev/docker-compose.yml up
```

