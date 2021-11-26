# WP Kickstarter
This is your project template to start with the `WP-CLI tool`.

## Related repositories and packages

### `joskoomen/wp-cli`
- WP-CLI is the actual source for all commands. 
- All Commands are integrated in the `jkwp` file inside this kickstarter. 
- Add custom commands for a project inside the `app` folder
- Add new commands from `joskoomen/wp-cli` inside `jkwp`
- `jkwp` has php syntax ;)
- [Github Repo](https://github.com/joskoomen/wp-cli)
- [Composer package](https://packagist.org/packages/joskoomen/wp-cli)

## Getting started
`composer install && php jkwp create -i && php jkwp serve`

## WP Config
If you want to extend your `wp-config.php` file with more options:
👉 https://www.wpbeginner.com/wp-tutorials/useful-wordpress-configuration-tricks-that-you-may-not-know/
👉 https://wordpress.org/support/article/editing-wp-config-php/

## Debug
- Debug is possible with [Kint Debug helper](https://kint-php.github.io/kint/)
- Read their documentation for more info. It's like the Laravel `dd`;

## CLI Commands available

### Create local Wordpress
| Available  | Command | Description
|--|--|--
| ✅ | `php jkwp create`                   | Create a new WP local Instance
| ✅ | `php jkwp create --wpv=5.6.1`       | ⬆️ With fixed version
| ✅ | `php jkwp create --install`         | ⬆️ Install and activate plugins

<br>

### Plugin management
| Available  | Command | Description
|--|--|--
| ✅ | `php jkwp install`                  | Install plugins
| ✅ | `php jkwp require [pluginname ...]` | Add plugin / plugins
| ✅ | `php jkwp remove`                   | Remove plugins not listed in wordpress.json
| ✅ | `php jkwp remove [pluginname ...]`  | ⬆️ Remove the given plugin / plugins
| ✅ | `php jkwp update`                   | Update plugin versions inside wordpress.json based on installed plugins
| ✅ | `php jkwp list [pluginname ...]`    | list the available versions of a plugin

<br>

### Application management
| Available  | Command | Description
|--|--|--
| ✅ | `php jkwp serve` | Serve your application at http://localhost:11001
