# Ascend base site installer

Ascend project base site install recipe.

- Currently using Drupal 10


From <https://github.com/poppopstudio/ascend>
in a normal ddev
git clone <git@github.com>:poppopstudio/ascend.git
composer install
ddev drush si recipes/ascend_base

- for resource branch
ddev drush recipe modules/custom/ascend_resource/recipes/resource

- for audit branch
ddev drush recipe modules/custom/ascend_school/recipes/school
ddev drush recipe modules/custom/ascend_audit/recipes/audit

Then absolutely you must clear the cache!
