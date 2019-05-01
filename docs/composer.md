# Composer


## Troubleshooting

!!! note "Can not delete files"

    ```
    [RuntimeException]
    Could not delete web/core/modules/layout_builder/tests/modules/layout_builder_test/src/Plugin/Layout/LayoutBuilderTestPlugin.php:

    ```

    This is related to file ownership, see [Error “could not delete” with Composer on Vagrant](https://stackoverflow.com/questions/26216437/error-could-not-delete-with-composer-on-vagrant/46277405#46277405). Change ownership using `chown owner:owner -R .`


!!! note "Out of memory"
	
	```
	Fatal error: Allowed memory size of 1610612736 bytes exhausted (tried to allocate 23124288 bytes) in phar:///usr/local/bin/composer/src/Composer/Util/RemoteFilesystem.php on line 458   
	
	```

	Increase php memory limit. 

!!! note "Package depenency issue"
    
	```
Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - Installation request for sebastian/diff (locked at 2.0.1) -> satisfiable by sebastian/diff[2.0.1].
    - phpunit/phpunit 7.0.0 requires sebastian/diff ^3.0 -> satisfiable by sebastian/diff[3.0.0].
    - phpunit/phpunit 7.0.1 requires sebastian/diff ^3.0 -> satisfiable by sebastian/diff[3.0.0].
    - phpunit/phpunit 7.0.2 requires sebastian/diff ^3.0 -> satisfiable by sebastian/diff[3.0.0].
    - Conclusion: don't install sebastian/diff 3.0.0
    - Installation request for phpunit/phpunit ^7 -> satisfiable by phpunit/phpunit[7.0.0, 7.0.1, 7.0.2].

	```

```
$ composer remove phpunit/phpunit --dev
$ composer require phpunit/phpunit --dev

    ```
