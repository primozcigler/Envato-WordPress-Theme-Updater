Envato WordPress Theme Updater
==============================

WordPress library to enable automatic updates in the theme based on [Envato WordPress Toolkit Library](https://github.com/envato/envato-wordpress-toolkit-library) and [pixelentity PHP class](http://themeforest.net/forums/thread/simple-theme-update-class-using-envato-api/73278).

### Installation & Use

Download this archive to your theme, then add

	load_template( trailingslashit( get_template_directory() ) . 'wp-theme-upgrader/envato-wp-theme-updater.php' );
	Envato_WP_Theme_Updater::init( $username, $apikey, $author );

to your `functions.php` where

	$username = Buyer Username
	$apikey   = Buyer API Key
	$author   = Your Author Name (as defined in your themes style.css)

The first 2 parameters should be set by the buyer somehow, like in your theme options page.
`$author` variable can be a single name, like "Pixelentity" or an array of strings. If not set,
all themes purchased by the user on ThemeForest (even if by different authors) can be updated.

Enjoy!

Pixelentity Team & ProteusThemes.