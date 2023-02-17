# TUTORIAL NOTES:

| **Tutorial Name**    | **Create a WordPress Plugin from Scratch [Playlist]** |
| -------------------- | ----------------------------------------------------- |
| File Name            | README.md                                             |
| Date Created         | 02/17/23                                              |
| Date Modified        | --                                                    |
| Platform             | YouTube                                               |
| Channel              | Alessandro Castellani                                 |
| Version              | 0.0.1                                                 |
| Programmer / Student | **Eric Hepperle**                                     |

* **Tutorial URL:** https://www.youtube.com/watch?v=Z7QfH-s-15s

---

## Dev Environment

### Install New Local WordPress Site

- Discourage search engine visibility

## Video 1

- Set `WP_DEBUG` to **true** in **wp-config.php**: This ensures that any errors will be displayed on screen.
- **GOTCHA:** Only have this on during development -- Turn off before push to live / production!

```php
define('WP_DEBUG', true);
```

---

- Navigate to `wp-content/plugins` folder
- Create new folder - the folder name will be same as your main PHP file

**#TIP:** To avoid any plugin name conflicts, in the WP Dashboard > Plugins > Click "Add New" and search for the plugin name that you want. This will tell you what plugins are likely to conflict so that you can give yours a unique enough name.


- Create plugin folder **alecaddd-plugin**
- Inside plugin folder create main plugin file **alecaddd-plugin.php**
- Add the following to main plugin file contents:

  - Declare package name: AlecadddPlugin

Create comment block as follows:

|Field|Value|Purpose|
|-|-|-|
|Plugin Name:|Alecaddd Plugin||
|Plugin URI:|http://alecaddd.com/plugin|The website that the plugin calls home|
|Description:|This is my first attempt to write a custom Plugin for this amazing tutorial series.| Describe the plugin|
|Version:|1.0.0|Version number|
|Author:|Alessandro "Alecadd" Castellani|Author name|
|Author URI:|http://alecaddd.com|When the user clicks the author name, this is the website it will take them to|
|License:|GPLv2 or later|Use open source license|
|Text Domain:|alecadd-plugin|Same as folder name|

**#GOTCHA:** Author says it is hard to release a plugin on official WP repository that is not open source so best just to use a GPL license.

## Create New WordPress Install for tutorial

Database Name: **tut_loc_alecadd_20230217**




--- --- ---

## Questions

  - **Q:** _Why is @package even necessary? What does it do?_


## Cleanup

- Set `WP_DEBUG` to false
- Enable search engine visibility