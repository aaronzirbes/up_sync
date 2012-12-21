Up-Sync
=======

This is a Gradle script that will keep your GitHub upstream repositories in sync

Requirements
------------

* Gradle
* Git command line tools

Usage
-----

Initialization

This will initialize your `gradle.properties` and `settings.gradle` files.

    gradle buildSettingsGradle


Synchronization

This will synchronize your local and origin repositories with upstream, and merge upstream/develop with your local develop and active branches

    gradle sync

Pruning

This will delete branches from your origin and local repository that are not feature branches (start with 'feature/') and do not live in upstream

    gradle deletePrunedBranches

