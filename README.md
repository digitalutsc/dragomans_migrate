# Dragomans Migrate module

## Instllation 
* Install the module dependencies: [migrate_plus](https://www.drupal.org/project/migrate_plus), [migrate_tools](https://www.drupal.org/project/migrate_tools) and [migrate_source_csv](https://www.drupal.org/project/migrate_source_csv).
* Apply this patch for migration_plus: https://www.drupal.org/files/issues/migrate_tools_dashboard-2825846-4.patch (Download the module.  Make it a git repo.  Follow [this tutorial](https://www.devroom.io/2009/10/26/how-to-create-and-apply-a-patch-with-git/) to apply the patch.)
* Install the module
 
## Reviewing the migration info
* You can review the migration info from here: http://localhost:8000/admin/structure/migrate

## Executing migration tasks
### Import the Data
```
drush mi import_nations
```

### Rollback
```
drush m4 import_nations
```

### Migrate commands
* The full list of migration drush command is described here: https://www.drupal.org/docs/8/upgrade/upgrade-using-drush

