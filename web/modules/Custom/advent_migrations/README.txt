#Admin credentials
* UserName 'admin', Password '3twk3wasnc' .

# Migration from Drupal 7
* Ensure that **migrate_plus**, **migrate_tools** are installed and enabled.


## Migration Commands
* **drush ms --group insights** : This is to list all the migration scripts under the insights group.
* **drush mrs <script-name>** : This will reset the status of the migration with the given script-name. This is done if the migration failed for some reason. It will set the migration status to idle.
* **drush mim <script-name>** : This is to import a specific migration script.
* **drush mr <script-name>** : This is to rollback the script which was run previously.


## User Import
* **D7 Users** - ```drush mim insight_user```