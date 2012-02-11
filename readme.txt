=== Plugin Name ===
Contributors: GaryJ
Donate link: http://code.garyjones.co.uk/donate/
Tags: admin bar, genesis
Requires at least: 3.3
Tested up to: 3.3.1
Stable tag: 1.3.0

Adds resource links related to the Genesis Framework to the admin bar.

== Description ==

This plugin adds resources links related to the <a href="http://genesis-theme-framework.com/">Genesis Framework</a> to the admin bar.

These resources include direct links to StudioPress support forums for each theme, quick access to Genesis Theme and SEO settings pages, quick access to Genesis-related plugin settings pages (for those that are active), and links to useful tutorial pages for how to get the most out of Genesis.

The plugin is built with theme and plugin developers in mind, as they can add support for their product with only a few lines of code, giving their users instant access to the right support board, a link to *their* website etc.

* Adds support for menu item positioning, so custom entries can be added anywhere, and not just as the final items.
* Easy addition of Support board links via single lines in theme `functions.php`.

This plugin is conceptual fork of the Genesis Admin Bar Addition plugin, re-written from scratch, adding new features.

Please report issues at https://github.com/GaryJones/Genesis-Admin-Bar-Plus/issues and not the WP Forums.

== Installation ==

1. Unzip and upload `genesis-admin-bar-plus` folder to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Ensure you're displaying the admin bar (front and / or back-end) via the settings on the User Profile page.

== Frequently Asked Questions ==

= Can I add my own entries to the Genesis menus? =

Yes - there is an action hook to do this. See the *Add Custom Items* section.

= How do I add a link to a certain support board? =

The plugin currently recognises all of the child theme support boards, <a href="http://genesis-theme-framework.com/">Genesis</a>, the translations board, the general plugins board and the GenesisConnect board.
See the *Add Support Boards* section for an example of how to add these to the Support menu.

You can also add a reference to another board via the `gabp_support_boards` filter.

= What settings links are supported? =
The following theme and plugins, when active, have a link to their settings page added to the Settings submenu:

* Design Settings (for [Prose Theme](http://gmj.to/prose))
* [GenesisConnect](http://gmj.to/genesisconnect)
* [Genesis Simple Breadcrumbs](http://wordpress.org/extend/plugins/genesis-simple-breadcrumbs/)
* [Genesis Slider](http://www.studiopress.com/plugins/genesis-slider)
* [Genesis Simple Edits](http://www.studiopress.com/plugins/simple-edits)
* [Genesis Simple Hooks](http://www.studiopress.com/plugins/simple-hooks)
* [Genesis Simple Sidebars](http://www.studiopress.com/plugins/simple-sidebars)
* [Simple URLs](http://www.studiopress.com/plugins/simple-urls)

A plugin author can add support for their own settings page link. See the *Add Custom Items* section.

Genesis Simple Menus and Genesis Tabs can't be supported as they have no individual settings pages.

== Screenshots ==

1. Support menu expanded, to show 3 optional items added via theme `functions.php` using `add_theme_support()`
2. Codex menu expanded
3. StudioPress menu expanded, along with FAQ submenu, and with debug mode enabled to show calculated menu positions
4. Settings menu expanded, showing support for direct link to settings pages of several Genesis-related plugins
5. Showing the StudioPress menu item removed, Support menu item moved position and new custom menu items added

== Changelog ==

= 1.3.0 =
* Added Italian language files to the plugin (props [http://gidibao.net/](Gianni Diurno))
* Added support for AgentPress 2, Backcountry, Balance, eleven40, Generate and Luscious themes.
* Added support for Clip Cart, Cre8tive Burst, Curtail, Driskill, Politica and Pure Elegance Marketplace themes.
* Improved icon markup and styles to match how WP 3.3 does it, which fixes overlapping icon issue.
* Improved properties and methods by declaring public or private visibility.
* Fixed to use new /tutorials links as StudioPress re-arrange their site.
* Fixed to use stricter code standards above and beyond WP CS.

= 1.2.5 =
* Added support for Fashionista, Modern Blogger (both Marketplace) and Scribble themes.
* Added updated German language files back in with the plugin (props [http://deckerweb.de/material/sprachdateien/genesis-plugins/](David Decker))
* Improved a few strings to use the plugin text domain to avoid conflicts.
* Improved readme descriptions.

= 1.2.4 =
* Added support for Nitrous and Legacy (Marketplace) themes.

= 1.2.3 =
* Added support for Genesis Slider plugin.

= 1.2.2 =
* Added support for various child theme support boards.

= 1.2.1 =
* Added styles for RTL languages.
* Removed German translation files, and included a link in the new Translation section of the readme.

= 1.2.0 =
* Added support for Genesis Simple Breadcrumbs plugin.
* Added support for Free Child Themes support board.
* Improved code to eliminate global constant and allow actions and filters to be unhooked by other plugins or functions.php.
* Removed two links due to StudioPress website re-organisation.
* Now requires PHP 5.

= 1.1.4 =
* Added support boards for newly-released Midnight and Blissful themes.
* Updated German translation.

= 1.1.3 =
* Fixed issue with sub sub menus, affecting FAQ links.
* Child menu items can now be added before parent items - the calculated positioning will add in the sum of all given ancestor item positions.
* Fixed confusing interface by styling non-links to use the default cursor.
* Updated all screenshots - now up to date, and considerably smaller file-size.
* Added explicit licensing of GPLv3.

= 1.1.2 =
* Fixed URLs from being echoed to bottom of admin pages.

= 1.1.1 =
* Added option to enter GABP Debug mode by appending `gabp-debug` as querystring argument.
* Fixed translation files by renaming them.
* Added a Codex suggestion, to check for translation files in `wp-content/languages/` first.

= 1.1 =
* Improved menu position - now each sub menu can start numbering items from 0, as child menu item will automatically be given a minimum position value of its parent.
* Added debug mode (uncomment line at top of plugin file). Can be used to show calculated menu position.

= 1.0.1 =
* Added further checks to see if plugin is active.
* Improved inconsistent external link icon by replacing CSS Unicode characters with base64 encoded image.
* Included .pot file for translations.
* Added German translation files (props [deckerweb.de](http://deckerweb.de/material/sprachdateien/genesis-plugins/)).
/)).
= 1.0 =
* First public version.

== Upgrade Notice ==

= 1.2.5 =
Minor changes - Improved strings for translations, add support for three themes, improved readme.

= 1.2.4 =
Minor changes - add support board for Nitrous and Legacy themes.

= 1.2.3 =
Minor changes - add support for Genesis Slider plugin.

= 1.2.2 =
Minor changes - add support boards for new themes.

= 1.2.1 =
Minor change - add styles for RTL support.

= 1.2.0 =
Several changes - add support for Genesis Simple Breadcrumbs plugin, free child themes board, improved code, removed two links. NOW REQUIRES PHP5.

= 1.1.4 =
Minor changes - add support boards for new themes, Midnight and Blissful.

= 1.1.3 =
Important changes if adding / modifying / removing menu entry.

= 1.1.2 =
Minor changes - remove echo from bottom of admin pages.

= 1.1.1 =
Minor changes - debug option, translation files.

= 1.1 =
Improved menu position calculation, added debug mode.

= 1.0.1 =
Minor changes - improved external link indicator, translation improvements.

= 1.0 =
Update from nothingness. You will feel better for it.

== Add Custom Items ==

Here's an example which removes the StudioPress menu (you only need to remove the parent item to remove all of the child items too), moves the Support menu item to the bottom of the submenu and adds some custom menu items in:

`add_action( 'gabp_menu_items', 'child_gabp_menu_items', 10, 3 );
/**
 * Amend the menu items in the Genesis Admin Bar Plus plugin.
 *
 * @param Genesis_Admin_Bar_Plus_Menu $menu
 * @param string $prefix
 * @param string $genesis
 */
function child_gabp_menu_items( $menu, $prefix, $genesis ) {
	$garyjones = $prefix . 'gary-jones';

	// Remove StudioPress item
	$menu->remove_item('studiopress');

	// Add Gary Jones item
	$menu->add_item( 'gary-jones', array(
		'parent'   => $genesis,
		'title'    => 'Gary Jones',
		'href'     => 'http://garyjones.co.uk/',
		'position' => 30
	) );

	// Add Gary Jones submenu items
	$menu->add_item( 'code-gary-jones', array(
		'parent'   => $garyjones,
		'title'    => 'Code Gallery',
		'href'     => 'http://code.garyjones.co.uk/',
		'position' => 10
	) );
	$menu->add_item( 'garyj', array(
		'parent'   => $garyjones,
		'title'    => 'GaryJ',
		'href'     => 'http://twitter.com/GaryJ',
		'position' => 20
	) );

	// Amend position of Support menu item - child items will move correctly too
	// as of v1.1
	$menu->edit_item( 'support', array(
		'position' => 50
	) );
}`

== Add Support Boards ==

To a add a reference to a support board (perhaps for the child theme the active theme is based on, or a plugin the site uses, etc), you can add something like one of the following to the child theme `functions.php` file.
`add_theme_support('gabp-support-genesis'); // Adds direct link to Genesis support board
add_theme_support('gabp-support-pretty-young-thing'); // Adds link to Pretty Young Thing child theme support board
add_theme_support('gabp-support-prose');  // Adds link to Prose child theme support board
add_theme_support('gabp-support-focus'); // Adds link to Focus child theme support board
add_theme_support('gabp-support-translations'); // Adds direct link to Genesis Translations support board
add_theme_support('gabp-support-plugins'); // Adds direct link to StudioPress Plugins support board
add_theme_support('gabp-support-genesisconnect'); // Adds direct link to GenesisConnect support board`
For child themes, the bit after the `gabp-support-` string must be the theme name, lowercase, with spaces replaced with hyphens.

== Translations ==

* Deutsch: http://deckerweb.de/material/sprachdateien/genesis-plugins/#genesis-admin-bar-plus
* Italiano: http://gidibao.net/
