# Example of no-ff merges

## Master branch

`master` branch with a linear history:

![master](./images/master.png "Master branch")

## Development branch

`master` branch is periodically merged to `dev` branch.

```shell
git checkout dev
git merge --no-ff master
```

![dev](./images/dev.png "Development branch")

## Test branch

`dev` branch is periodically merged to `test` branch.

```shell
git checkout test
git merge --no-ff dev
```

![test](./images/test.png "Test branch")

## Production branch

`test` branch is periodically merged to `prod` branch.

```shell
git checkout prod
git merge --no-ff test
```

![prod](./images/prod.png "Production branch")

## All branches

![all](./images/all.png "All branches")
