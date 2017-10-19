# Heroku Buildpack: Go Migrate

This is the [Heroku buildpack][buildpack] for migrations that use [mattes/migrate][go-migrate].

## Usage

The following environment variables must be set:
1. `MIGRATE_PATH` - the path to the directory that has the migrations (will be provided as the `-path` flag to the migrate command)
2. `MIGRATE_DATABASE_URL` - the database url in the correct format (e.g. [mysql url format][go-migrate-mysql])

[buildpack]: http://devcenter.heroku.com/articles/buildpacks
[go-migrate]: https://github.com/mattes/migrate
[go-migrate-mysql]: https://github.com/mattes/migrate/tree/master/database/mysql