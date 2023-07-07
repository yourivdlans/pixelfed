# Upgrading

## Update branches

```sh
git checkout dev
git pull upstream dev
git checkout dokku
git rebase dev
git push -f origin dokku
```

## Update dokku app

```sh
git push dokku dokku:master
```

## Run migrations

```sh
ssh dokku@projects.itflows.nl enter pixelfed web
php artisan migrate
```
