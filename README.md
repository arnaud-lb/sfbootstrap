Symfony standard + a few bundles

Added bundles:

- [FOSUserBundle](https://github.com/FriendsOfSymfony/FOSUserBundle)
- [MtHamlBundle](https://github.com/arnaud-lb/MtHamlBundle)

Install:

``` sh
git clone git://github.com/arnaud-lb/sfbootstrap.git
git submodule update --init
```

app/config/parameters.yml:

``` yaml
parameters:
  database_driver:   pdo_mysql
  database_host:     localhost
  database_port:     ~
  database_name:     sfbootstrap
  database_user:     root
  database_password: ~

  mailer_transport:  smtp
  mailer_host:       localhost
  mailer_user:       ~
  mailer_password:   ~

  locale:            en
  secret:            ThisTokenIsNotSoSecretChangeIt
```

Create db tables:

``` sh
./app/console doctrine:schema:create
```

