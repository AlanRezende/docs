---
title: Installation
icon: fal fa-arrow-alt-to-bottom
---

Install everything at once using composer.

```bash
composer require tenancy/tenancy
```

## Framework

Instead of loading the framework and all drivers at once, you can selectively install
what you need. You need at least the framework:

```bash
composer require tenancy/framework
``` 

After that add the database and identification drivers you need.

### Database

Load the database driver package for the database you are using, eg;

```bash
composer require tenancy/db-driver-mysql
```

Check the documentation on [database drivers][db-drivers] to find a suitable package
for your app. 

### Identification

The next step in setting up, is to install a tenant identification driver. Comparable
how database connections are set up, tenancy allows you to configure any number of
identification drivers.

Install the default http identification driver:

```bash
composer require tenancy/identification-driver-http
```

More drivers and information to write your own can be found in the section about
[identification drivers][identification-drivers].

You are now set up. Move to the next article to configure your application and set
up your first tenant!


[db-drivers]: database-drivers
[identification-drivers]: identification-drivers
