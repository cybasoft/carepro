# Installation

> Built using CodeIgniter 3.1.6 so familiarity with the framework is a plus

## Requirements

* PHP >= 7.0

* MySQL >=5.5

* SSH access (optional for remote installation)

* Command line access (CLI)

## Quick steps

> Assuming this is new installation or complete re-install (all previous data is lost)
1. Copy all files to your install directory
1. Edit index.php and change APP_ENV from `development` to `production`
1. Edit application/config/database.php and add your database credentials
1. Edit application/config/config.php and add URL of your installation e.g. `http://example.com/` &longleftarrow; note the trailing slash.
1. Open terminal from root of your application and run `php index.php migration run`
> If this is a fresh re-install, you can run `php index.php migration refresh' to overwrite the entire database

1. Login to your app using `admin@app.com/password`

## Detailed steps

* Copy all application files to the desired installation directory

* For upgrades, you can skip overwriting `/system` directory. You can also skip any existing directory inside `/assets/plugins`.
* Create a database
* Open `application/config/production/database.php` and add your database credentials

* Open `application/config/production/config.php` and update your installation settings

If  you are on development/testing server, create the respective directories and copy the database.php and config.php there.

* Run `php index.php migration run` to run a new migration copy or just `php index.php migration run <version number>`  to upgrade to the latest migration.
*`php indx.php migration run`, you will need to confirm by typing in production mode "yes"
* `composer install` install dependencies
* Run `php index.php migration seed` to run all available seeds or `php index.php migration seed SeederClass` where SeederClass is the name of the seeder file. Ommit the numeric portion '00_' and extension '.php'.

Available seeders:

`UsersTableSeeder`
`GroupsTableSeeder`
`NewsTableSeeder`
`RoomsTableSeeder`
`CalendarTableSeeder`

> IMPORTNANT! Remember to set your application to production in index.php when setup is complete! You can also set environment in your .htaccess by adding `SetEnv CI_ENV production`

After seeding, you will have a default admin user to login into your application for the first time.

> Email: admin@app.com
<!-- . -->
> Password: password

> IMPORTANT! Remember to reset the password for the default admin account!

> You can reload migrations by running `php index.php migration refresh`. You must be in development environment. All data will be lost

> You can undo the last migration by running `php index.php migration undo`

## Advanced

### For developers

1. Run `composer install` to install dependencies
1. Open `application/models/Conf.php` and set `ENVIRONMENT="development"` in the debug section