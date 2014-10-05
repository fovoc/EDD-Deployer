EDD-Deployer
============

## Warning: This plugin is still under development and currently does NOT work.


Remotely install plugins and themes. The package consists of a plugin that has to be installed on a server running EDD (and optionally EDD-SL) and a demo plugin for the client sites.

# Usage:

### Server-side:

Install and activate the plugin.

### Client-side:

This is still under heavy development and we would not recommend its use for production purposes.

```php
<?php

$edd_deploy_client = new EDD_Deploy_Client( 'http://example.com' ); // The URL of our site running EDD
$installation_url  = $edd_deploy_client->install_url( 'plugin', 'Plugin Name' );
?>
```
The above will create a URL that will automatically download the plugin from our remote server and install it.

You can simply install the client plugin on a site, change the array containing the downloads and then don't forget to change the URL (http://example.com) to your own.

This has only been tested so far with free plugins.
