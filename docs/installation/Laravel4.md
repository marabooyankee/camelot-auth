### Installing in Laravel 4 (with Composer)

##### Step 1
Start by adding " t4s/camelot-auth": "*" to the require attribute in your composer.json file.

```javascript
{
	"require": {
		"t4s/camelot-auth": "*"
	}
}
```

Alternatively, you can issue the following in the terminal:

```
	$ php composer.phar require t4s/camelot-auth
```

##### Step 2
Run `php composer.phar update` from the command line  

##### Step 3
Add `'T4s\CamelotAuth\CamelotAuthServiceProvider'` to the `providers` array in app/config/app.php

##### Step 4
Add `'Camelot' => 'T4s\CamelotAuth\Facades\Camelot',` to the `aliases` array also in app/config/app.php

##### Step 5
Publish configurations:

```
	$ php artisan publish:config ts4/config
```

Now you can setup one of the [Authentication drivers](https://github.com/taftse/camelot-auth/wiki#driver-setup)