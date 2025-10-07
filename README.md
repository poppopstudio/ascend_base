# Ascend base site installer

Ascend project base site install recipe.

- Currently using Drupal 10

in a normal ddev:
git clone <git@github.com>:poppopstudio/ascend.git
composer install
ddev drush si recipes/ascend_base

- for resource branch
ddev drush recipe modules/custom/ascend_resource/recipes/resource

- for audit branch
ddev drush recipe modules/custom/ascend_audit/recipes/audit

** Then you absolutely must clear the cache! Twice is nice :)

- if you need demo data (which is out of date atm)

  - delete folders: ascend_demo_data/content/[cluster, rating, user, school] if using only resource
  - delete folders:  " /[pricing, stage] if using only audit branch

then
ddev drush recipe ../recipes/ascend_demo_data
