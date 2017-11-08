# Dragomans Migrate module

## Introduction

Dragomans Migrate is a Drupal 8 module that is used to migrate CSV spreadsheet metadata from the Dragomans Renaissance Research project into Drupal nodes. Please see the [wiki](wiki) for more information.

## Installation

* Install the module dependencies: [migrate_plus](https://www.drupal.org/project/migrate_plus), [migrate_tools](https://www.drupal.org/project/migrate_tools) and [migrate_source_csv](https://www.drupal.org/project/migrate_source_csv).
* Apply this patch for migration_plus: https://www.drupal.org/files/issues/migrate_tools_dashboard-2825846-4.patch (Download the module.  Make it a git repo.  Follow [this tutorial](https://www.devroom.io/2009/10/26/how-to-create-and-apply-a-patch-with-git/) to apply the patch.)
* Install the module dragomans_migrate

## Reviewing the migration info

* You can review the migration info from here: http://localhost:8000/admin/structure/migrate

## Executing migration tasks
### Import the Data

```
drush mi import_nations
```

### Rollback

```
drush mr import_nations
```

### Migrate commands

* The full list of migration drush command is described here: https://www.drupal.org/docs/8/upgrade/upgrade-using-drush

## References

* https://www.mtech-llc.com/blog/lucas-hedding/migrating-using-csv
* https://evolvingweb.ca/blog/drupal-8-migration-migrating-basic-data-part-1
* https://www.mtech-llc.com/blog/ada-hernandez/entity-lookup-generate-migrate-process-plugins (inline entity lookup)
* https://www.drupal.org/node/2825565 (multi value fields)

## Maintainers

* Natkeeran Ledchumykanthan
* Marcus Barnes
