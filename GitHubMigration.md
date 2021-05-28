## Migrate your repository by using GitHub best practices

* If you want to retain version control history, then you will need to import using the `GitHub Migrator tool`. See [Importing data from third-party version control systems](https://help.github.com/enterprise/2.20/admin/migrations/importing-data-from-third-party-version-control-systems).
* Beyond Git data, you may also have a desire to retain issues, pull requests, or other data. Support for these items will vary by platform and is generally available from community projects.
* Avoid committing large binary files, such as build artifacts. If you have a need to version large binary files, consider using the Git extension `Git LFS` (Large File Storage).