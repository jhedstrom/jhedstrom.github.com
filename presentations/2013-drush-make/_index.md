## drush[make]

    api = 2
    core = "7.x"
   
    projects[ctools][version] = "1.3"
    ; http://drupal.org/node/1120028#comment-5792282
    projects[ctools][patch][] = "http://drupal.org/files/patch-1.patch"
    ; https://drupal.org/node/1417630#comment-6810906
    projects[ctools][patch][] = "https://drupal.org/files/patch-2.patch"

## New for 6.x
### (most backported to 5.x)

## Local patches
### (patch copied into project directory)

## Use a distribution as core

    core = 7.x
    projects[commerce_kickstart][type] = "core"
    projects[commerce_kickstart][version] = "7.x-1.19"

## Quick Drupal can use a makefile

   ```
   drush qd --makefile=mysite.make
   ```

## Per-project working-directory

    projects[caption_filter][download][revision] = "c9794cf"
    projects[caption_filter][download][working-copy] = 1

## Set defaults

    defaults[projects][subdir] = "contrib"
   
instead of
   
    projects[foo][subdir] = "contrib"
    projects[bar][subdir] = "contrib"
