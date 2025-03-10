# Shariff Wrapper

This is the development repository for the WordPress plugin Shariff Wrapper (https://wordpress.org/plugins/shariff/), which has been developed by Jan-Peter Lambeck (https://www.jplambeck.de) and 3UU (https://datenverwurstungszentrale.com).

/shariff/ = The actual WordPress plugin.  
/assets/ = Files used on the wordpress.org plugin page.  

license.txt = The license file (MIT).  
readme.md = This file.  
shariff-example-service.php = Example file for new services.

## Contribute

Pull requests are more than welcome, especially for new services. You can use the shariff-example-service.php to get started. All service specific elements need to be included in this file. Please always create a separate pull request for each service, feature or bug fix.

Please follow the WordPress Coding Standards (https://make.wordpress.org/core/handbook/best-practices/coding-standards/) in general for ALL pull requests and especially the PHP Coding Standards (https://make.wordpress.org/core/handbook/best-practices/coding-standards/php/).

If you need any help or have specific questions regarding development and contribution, simply open up an issue and we will try to help you. For support requests about the plugin itself please use the WordPress Support Forum (https://wordpress.org/support/plugin/shariff).

## Changelog

= 4.6.9 =
- new service Mastodon (thanks to Nikita @kytta@fosstodon.org by providing s2f.kytta.dev)
- updated LinkedIn share link

= 4.6.8 =
- updated to Facebook Graph API v15.0
- removed deprecated services Flattr, QZone and TencientWeibo
- removed Twitter share counts via Twitcount
- removed broken links from help tab

= 4.6.7 =
- updated to Facebook Graph API v11.0
- changed FB request to og_object (thanks to richard67)

= 4.6.6 =
- Fix sanitize_callback parameter to avoid warnings with api requests
- tested for 5.7

= 4.6.5 =
- updated to Facebook Graph API v6.0
- fixed minor bug
- tested for WordPress 5.4

= 4.6.4 =
- fixed the settings link on the plugin overview page for certain environments (thanks to @midgard)
- updated to Facebook Graph API v5.0
- updated the WhatsApp link to swap url and title for a working image preview
- removed nofollow from the info button
- remvoed Xing share counts due to Xing disabling the API

= 4.6.3 =
- updated the WhatsApp share link to work with all devices again (thanks to @hanshansenxxx)
- updated to Facebook Graph API v3.3
- updated the Flattr button to reflect the new Flattr (thanks to Chris, @camthor)
- fixed an update issue with WP CLI
- removed the Facebook share counts request without APP ID and Secret
- Facebook now always requires an APP ID and Secret for share counts
- removed Flattr counts due to Flattr removing the API

= 4.6.2 =
- new service MeWe
- new service Buffer
- fixed an issue in case the plugin dir has been moved via symlink

= 4.6.1 =
- replaced Stumbleupon with its successor Mix (thanks to Mark)
- added an option to hide WhatsApp on desktop devices
- updated Odnoklassniki API
- fixed an issue with WPML and some older Shariff setups

= 4.6.0 =
- new high contrast theme (WCAG)
- improved support for WPML for easier translation of headlines and info button texts
- updated WhatsApp share link to support WhatsApp Web (thanks to Oliver, @oliverpw)
- updated Spanish translations (thanks to Torsten, @torstenbulk)
- updated Pinterest Share Count API
- updated VK Share Count API
- updated Pocket API
- updated XING API
- removed GooglePlus due to Google shutting GooglePlus down
- fixed a PHP notice in regards to Tumblr (thanks to Mario, @mariobartlack)
- fixed a conflict with another plugin (thanks to David, @daveshine)
- tested with WordPress 5.1

= 4.5.3 =
- removed LinkedIn Share Counts due to LinkedIn removing them completely
- removed GooglePlus Share Counts due to Google shutting GooglePlus down
- removed OpenShareCount due to the service having shut down
- removed NewShareCount due to the service having shut down
- removed Mastodon temporarily until a new working solution is available
- deprecated GooglePlus as a service, will be removed with the next release
- added TwitCount (twitcount.com) as an alternative for Twitter share counts
- updated to Facebook Graph API v3.2
- updated to WordPress Coding Standards 2.0
- corrected minor typos
- added the new logo thanks to Philipp Wildfeuer (@phil_sauvage)

= 4.5.2 =
- added support for share count requests of multilingual sites
- updated button translations for Twitter and Pinterest (thanks to Jessica, @jess78)
- updated to Facebook Graph API v3.0

= 4.5.1 =
- added support for the new WordPress Privacy Policy Guide added in 4.9.6
- minor css adjustments
- minor bug fixes

= 4.5.0 =
- new option to add Shariff to custom WordPress hooks
- new option to support multilingual sites using WPML and other plugins
- new support for WooCommerce products on the ranking table
- new option to show different headlines based on share counts
- updated button languages, now supporting 25 languages
- fixed a bug causing share counts to not being displayed properly

= 4.4.4 =
- add support for automatic addition to bbpress forums, topics and replies
- fix a bug that caused "hideshariff" to not function properly

= 4.4.3 =
- new support for additional manual AMP integrations
- fixed a PHP error on certain server configurations
- new support for the print button on AMP pages
- fixed a markup typo
- minor css improvements

= 4.4.2 =
- new support for the "AMP for WP" plugin by Ahmed and Mohammed Kaludi
- improved support for the "AMP for WordPress" plugin by Automattic
- new additional workaround for servers without $_SERVER for category pages
- minor bug fixes

= 4.4.1 =
- new service wallabag (thanks to Torsten, @knodderdachs)
- minor bug fixes
- updated help section

= 4.4.0 =
- new service Telegram (thanks to Daniel Sturm, @dcsturm)
- new service Flipboard (thanks to csigncsign, @csigncsign)
- new service Mastodon (thanks to scroom, @scroom)
- new service Qzone
- new service Weibo
- new service TencentWeibo
- new service SMS (will work on iOS, might not work on other phones)
- new support of the "AMP for WordPress" plugin by Automattic
- new option to set a custom text for the info button
- new option to disable the metabox
- new option to add shariff to CPTs before the content
- new ranking table now also shows pages
- new fix to prevent Shariff buttons from being displayed on admin pages
- new fix to support WP-CLI (thanks to Daniel Jagszent, @d--j)
- fixed HTML errors regarding self closing tags (thanks to Tooni, @tooni)
- fixed a missing closing tag under certain conditions (thanks to Pat, @fortythousandmiles)
- removed GooglePlus share counts due to Google removing the API
- added Czech translation of the buttons
- updated a lot of button translations
- updated to Facebook Graph API 2.12
- updated a lot of strings to allow for easier translation
- updated the reddit icon
- updated help section
- improved documentation of the REST API endpoint for share counts (thanks to David)
- major improvements in regards to code quality
- minor css improvements
- minor security improvements
- removed the mail form due to technical and legal due diligence
- if you need the mail form functionality, please stick to version 4.3
- https://downloads.wordpress.org/plugin/shariff.4.3.0.zip

= 4.3.0 =
- new service Odnoklassniki (thanks to rockhit)
- new meta box allows for individual settings per post or page
- new option to hide share counts that are zero
- new option to disable dynamic cache lifespan (not recommended)
- new option to set the button size to small, medium or large
- new option to add a custom class to the container around Shariff
- new option to open links in a popup (thanks to jackennils)
- new option to use NewShareCount instead of OpenShareCount (Twitter)
- added timestamp variable to be accessible via shortcode
- fixed post timestamp for caching under certain conditions
- fixed Facebook share count error for never crawled pages
- fixed empty tab after sharing on certain mobile devices
- fixed custom title attribute (thanks to kschlager)
- updated Flattr user id for the future (thanks to poetaster)
- reduced changelog on wordpress.org (thanks to timse201)
- minor css improvements
- updated help section

= 4.2.1 =
- fix WhatsApp button on Android when using Chrome
- fix Shariff being added to RSS feeds under certain conditions
- update to latest Facebook Graph API for share count requests

= 4.2.0 =
- new option to set the rate limit for sending mails using the mail form
- added home url as fallback for share count requests
- added further anti-spam prevention mechanics
- added noopener and noreferrer to share links
- fixed double encoding of share count request links
- updated media uploader request for translation
- updated handling of admin notices following WordPress core
- tested and optimized for WordPress 4.6

= 4.1.2 =
- new fallback for share count requests in case pretty permalinks are disabled
- new filter shariff3UU_render_atts to change options on the fly (thx Ov3rfly)
- fix share title in cases with html encoded characters
- fix double counting on ranking tab under certain conditions
- fix php info notice in admin notices

= 4.1.1 =
- new option to disable the Shariff buttons outside of the main loop
- fix Facebook App ID request
- minor css fix

= 4.1.0 =
- new design option to set a custom button color for all buttons
- new design option to set a border radius for the round theme (up to a square)
- new design option to hide all buttons until the page is fully loaded
- new mailform option to use a html anchor (again)
- new statistic option to fill the cache automatically
- new statistic option to set the amount of posts for the ranking tab
- new statistic option to use share counts with PHP < 5.4
- fix preventing buttons from beeing added to excerpts under certain conditions
- fix url encoding of share count requests
- improved handling of wrong or mistyped service entries
- minor bug fixes

= 4.0.8 =
- new workaround for sites running PHP 5.2 and older

= 4.0.7 =
- new option for WordPress installations with REST API not reachable in root

= 4.0.6 =
- fix error in combination with bbpress
- fix error on very old PHP versions
- fix ranking tab
- minor css improvements

= 4.0.5 =
- fix mail form link
- fix xmlns for w3c

= 4.0.4 =
- removed some remaining wrong text domains for translations
- minor css fixes

= 4.0.3 =
- fix mobile services not showing on certain tablets
- fix type error on totalnumber when cache is empty
- fix share count requests when WordPress is installed in a subdirectory
- fix urlencoding of share url, title and media
- add width and height to SVGs to prevent large initial icons prior to css
- new classes shariff-buttons and shariff-link added
- removed local translation files due to switching to wordpress.org language packs
- minor css resets added

= 4.0.2 =
- added minor css resets to prevent influence of theme css
- fixed LinkedIn share link

= 4.0.1 =
- prevent php warning messages on unsuccessful includes while WP_DEBUG is active
- change text domain to match plugin slug

= 4.0.0 =
- complete overhaul of the plugin core
- buttons now also work without JavaScript
- icon font has been removed and replaced with SVGs
- share counts now use the WP REST API
- share counts now always show the last cached counts prior to updating them
- fixed duplicated share count requests
- new ranking tab shows the shares of your last 100 posts
- new service pocket
- new option to show the total amount of shares in the headline with %total
- new option to use the total amount of shares in your theme (see FAQ)
- new action hook shariff_share_counts (see FAQ)
- new option to change the priority of the shortcode filter
- new support for selective refresh introduced in WP 4.5
- new external API feature replaces the external host option (experimental, see FAQ)
- new support for SCRIPT_DEBUG
- css and js files are now only loaded on pages with Shariff buttons
- improved compatibility with plugin Autoptimize (force scripts in head)
- improved compatibility with multiple caching plugins
- all shortcodes are now being stripped from the mail message body
- fixed potential double sending of mails
- removed all jQuery dependencies
- requires at least WordPress 4.4 (only for share counts)
- we no longer support IE 8 (if it ever worked)
- updated status tab
- updated help section
- minor bug fixes
- code cleanup

= 3.4.2 =
- fixed share counts on mobile devices with exactly 360px width
- fixed error on the help tab regarding services (thx to Andreas)
- small css improvements
- added h4-h6 to the allowed tags for the headline

= 3.4.1 =
- changed diaspora share url to official one
- fixed css of rss button when using round theme in widget
- fixed accessibility of share button text 
- added rssfeed option to help section
- updated to Heise version 1.23.0

= 3.4.0 =
- new service rss
- minor bug fixes
- update to Heise version 1.22.0

= 3.3.3 =
- fix anonymous function request for PHP < version 5.3

= 3.3.2 =
- improve/extend handling of custom post types
- fix Facebook ID call

= 3.3.1 =
- fix ttl setting on statistic tab
- reduce timeout for post requests to five seconds

= 3.3.0 =
- new option to use an external host for Shariff and the share count backend
- new share count service OpenShareCount.com for Twitter
- new settings tab "Statistic" for all options regarding the share counts
- new settings tab "Status" for all system checks to increase performance
- new design preview button without Twitter
- fix counter VK on design round
- fix Facebook total_count again
- fix double Twitter share windows under certain conditions
- reactivate Flattr counts, since they fixed their API
- purge Shariff transients on update, deactivate and uninstall
- code cleanup
- add vk to help section
- add a known bugs section to the readme

= 3.2.0 =
- new service VK
- new share count service VK
- new dynamic cache lifespan (ttl) based on post / page age (last modified)
- new option to disable individual services (only share counts)
- fix Facebook share counts now use total_counts again
- fix search for custom WP locations
- backend optimization
- temporarily disabled the Flattr counts (statistic) due to ongoing problems of the Flattr API
- fix use of wp_title() is/was deprecated in WP4.4

= 3.1.3 =
- fix ajax call when a custom permalink structure is used

= 3.1.2 =
- fix Facebook ID on 32-bit systems

= 3.1.1 =
- make admin help compatible to the new backend

= 3.1.0 =
- new option to add buttons before/after the excerpt
- new service Threema (thanks to medienverbinder)
- new service Diaspora (thanks to craiq)
- new service AddThis (thanks to bozana)
- new share count service AddThis (thanks to bozana)
- new service PayPal.Me
- new google icon
- fix title tag usage in some cases
- fix rel to data-rel popup
- fix round buttons in certain themes
- fix Flattr API to fetch counts again
- workaround to fix the wrong JSON answer of xing API
- up to date with Heise code version 1.21.0 2015-11-06

= 3.0.0 =
- new WP specific statistics backend for share counts
- new SHARIFF_WP_ROOT_PATH constant for custom wp locations
- automatic search for custom WP locations (thanks to hirasso)
- fix timeout issues and a lot of other backend issues
- deprecated Heise shariff-backend-php
- deprecated ZendFramework
- deprecated shariff3uu_cache directory
- deprecated SHARIFF_BACKEND_TMPDIR constant

= 2.4.3 =
- fix proxy settings
- fix PHP error notice caused by a race condition around concurrent requests in Zend_Cache
- fix PHP notice and error in backend on multisite

= 2.4.2 =
- fix lang attribute again
- fix update notice

= 2.4.1 =
- fix lang attribute
- nicer support hints about GD lib
- cleanup readme.txt

= 2.4.0 =
- ensure compatibility to WordPress 4.3
- new service Tumblr
- new service Patreon
- new service PayPal
- new service Bitcoin
- new supporting bbpress
- new using proxy settings from wp_config (thanks to Shogathu)
- fix automatic button language
- fix button language for Facebook
- fix problems with plugin "Hide Title"
- fix backend (statistic) for multisite environments
- fix backend (statistic) if WP_DEBUG is set to true
- fix language info in help section
- update to Heise version 1.16.0
- remove unnesseray guzzle docs

= 2.3.4 =
- add Italian language to the mailform

= 2.3.3 =
- fix Pinterest button, if pinit.js is present
- small css fixes

= 2.3.2 =
- add French (thanks Charlotte) and Italian (thanks Pier) translations
- improve screen reader compatibility
- fix: prefill mail_comment in case of an error
- fix: do not send more than 1 email as CC. Use a new mail for all recipients.
- fix: fallback to English at the email form only if language is not supported by this plugin
- cleanup mf_wait + extend time to wait of robots blocker to 2 sec 

= 2.3.1 =
- fix facebook api (app id & secret)
- fix CSS mailform label

= 2.3.0 =
- redesing of the plugins options page
- mail form improved (a lot)
- split mail into mailform and mailto (check your manual shorttags!)
- new backend status section
- new option to use Facebook Graph API ID in case of rate limit problems
- new option to stretch the buttons horizontally
- new option to add a headline above the Shariff buttons
- many new button languages
- new default cache directory
- fix creation of default cache directory in case it is not month / year based
- fix url-shorttag-option in widget
- fix widget mailform link, if pressed twice
- fix widget mailform on blog page
- fix responsive flow of buttons in IE
- fix Twitter: prevent double encoding with text longer than 120 chars
- update shariff backend to 1.5.0 (Heise)
- update shariff JS to 1.14.0 (Heise)
- many more minor improvements
- code cleanup

= 2.2.4 =
- security fix

= 2.2.3 =
- extend blocking of shariff buttons within password protected posts

= 2.2.2 =
- allow email functionality only if service email is configured within the
  admin menu as common service for all posts

= 2.2.1 =
- "fix" fallback to old twitter api again

= 2.2.0 =
- add option to hide Shariff on password protected posts
- tested up to WP 4.2.2
- "fix" fallback to old twitter api if another twitter script is found in order to avoid opening the share window twice
- share text of the mailto link now is "email"
- fix typo and cleanup code

= 2.1.2 =
- fix to make it work with PHP < 5.3 (you should really update your PHP version or change your hoster)

= 2.1.1 =
- change code because of a error with some PHP versions

= 2.1.0 =
- replace sender name if a name is provided with the mail form or set in admin menu
- add option to append the post content to the mail
- add mail header "Precedence: bulk" to avoid answers of autoresponder
- fix: rename a function to avoid problems with other plugins
- improve css

= 2.0.2 =
- fix: mail URLs must be a real link and not url-encoded
- hotfix: mail form disabled if not on single post. Avoid the 
  self destruction by the DOS-checker ;-)
- cleanup Shariff JS code (mailURL no longer needed)

= 2.0.1 =
- fix email form method POST

= 2.0.0 =
- changes to stay compatible to Heise implementation
- remove obsolet SHARIFF_ALL_POSTS
- fix some small css attributes (size)
- code clean up

= 1.9.9 =
- fix widget bug (wrong share links)

= 1.9.8 =
- add headers to avoid caching of backend data
- tested with WP 4.2 beta
- add option to use on custom pages (e.g. WooCommerce)
- better handling of pinterest media attribute
- bugfix: SHARIFF_BACKEND_TMPDIR in backend
- improve uninstal of cache dir (todo: change to a better named dir)
- add option to use smaller size buttons
- fix again target of the mailto-link
- cleanup code

= 1.9.7 =
- roll back to stable

= 1.9.6 =
- now really go back to 1st block in loop at WMPU

= 1.9.5 =
- nu abba: missing version update 

= 1.9.4 =
- fix update bug on WPMS

= 1.9.3 =
- add missing backend files. Last change for this Sunday ;-)

= 1.9.2 =
- fix stupid bug with the update file :-( Sorry!
- fix initialisation of REMOTEHOSTS 

= 1.9.1 =
- merge with original Shariff JS/CSS code version 1.9.3
- CSS theme default like Heise default again + "add" theme color
- fix the theme "white"
- backend now up to date
- disable WPDebug in backend config
- improve uninstall (options shariff3UU, shariff3UUversion,
  widget_shariff) and compatible with multisite installations
- improve deactivation

= 1.9 =
- add Flattr
- improve version control
- update frensh translations
- use configuration from admin menu for blank shariff shortcodes
- own (much smaller) fonts

= 1.8.1 =
- remove the relativ network-path from service declarations (pinterest,
  reddit, stumbleupon, xing) because it really makes no sense to change 
  the protocol within a popup of a secure target to unsecure connections
  depending on the protocol the page is using
- change name of jQuery object to avoid conflicts with other plugins/themes

= 1.8 =
- add options to place Shariff (right/left/center)
- fix: migration check
- css optimized
- use the WP bundled jQuery now (save about 80% bandwidth :-)

= 1.7.1 =
- optimize css (thanks again to @jplambeck)
- code cleanup (No more warnings in debug mode. Perhaps ;-)
- sanitize admin input (thanks again to @jplambeck)
- set the title attribute to overwrite get_the_title() now supported
- fix: check SHARIFF_BACKEND_TMPDIR
- add uninstall script

= 1.7 =
- CHANGES: if no attributes are configured within a shorttag first try to
  use the option from admin page. However if there are no services
  configured use the old defaults of Heise to make it backward compatible
- add the new service attribut `mailto` to prepare getting the original
  behavior of the Heise code that provide a email form with `mail`
- add option to put Shariff on overview page too
- add internal version tracker to enable better migration options in the
  future
- optimized css for the info attribute, added priority to the title
  attribute over DC.title attribute (thanks again to @jplambeck )

= 1.6.1 =
- fix: again enable WhatsUp on mobile now also works with Mozilla. Sorry
  this has not been become part of the main branche. Therefor it was lost 
  with the last update :-(
- added .shariff span { color: inherit; } (thanks again to @jplambeck )

= 1.6. =
- adopted new responsive css code (thanks to @jplambeck )
- update included fa-fonts
- fix: descrition "printer" 
- fix: use WP_CONTENT_URL in admin menu

= 1.5.4 =
- remove alternativ css with links to external hosters. If do you really
  want enable breaking privacy plz feel free to code you own css 

= 1.5.3 =
- hide counter within the theme round 

= 1.5.2 =
- default backend temp dir now uses wp content dir 
- updated original shariff JS code

= 1.5.1 =
- fix: constant had have a wrong declaration check

= 1.5.0 =
- add option "url" to set a fixed URI for all sites (only in shorttag and
  widgets) because usually it is not a good idea to manipulate this
- fix: do not show error in elseif (/tmp check in admin menu) 

= 1.4.4 =
- add option to force frensh and spanish buttons
- clean up theme selection

= 1.4.3 =
- look like wp_enqueue_script has problems with the shariff js code. Now own
  script link at the end of the site. Should also improve performance ;-)

= 1.4.2 =
- fix: add the attribute data-title that is needed by the shariff on some
  themes to render it above the other div containers. 
- only long PHP-Tags because auf problems with WAMPs
- some code clean up. Hopefully it will become more robust on WAMP systems.

= 1.4.1 =
- fixed stupid typo with the SHARIFF_BACKEND_TMP constant

= 1.4.0 =
- add a DIV container to use positioning with CSS
- remove long PHP-tags that cause parse problem on Windows

= 1.3.0 =
- clean up the code
- add backend options (TTL and temp dir)

= 1.2.7 =
- fixed: enable WhatsUp on mobile now also works with Mozilla 
- print button does not open a new window
- removed min.js make it more readable for own local changes

= 1.2.6 =
- add print button
- add default image for pinterest to avoid broken design and giuve a hint

= 1.2.5 =
- hotfix for pinterest (see FAQ) 

= 1.2.4 =
- bugfix: widget does not work if SHARIFF_ALL_POSTS is set but not enabled
  in the admin menu (Please remember, that SHARIFF_ALL_POSTS will be 
  removed with next major version)
- add option to add shariff at the begin of a post
- merge with new original backend for counters
- add spanish language on buttons; hide whatsup on mobile devices
  (merge with yanniks code)
- add reddit
- add stumbleupon

= 1.2.3 =
- add round theme to the admin menu

= 1.2.2 =
- tested with WP 4.1
- added french language for buttons
- added theme "round" (round buttons without text but with fixed width)

= 1.2.1 =
- typos

= 1.2 =
- add widget support

= create a Stable1.0 tag =
- no new funtionality to this tag. Only bugfixes!

= 1.1.1 =
- add french language for the admin menu (thanks Celine ;-)
- fix backend problem on shared hosting with no writeable tmp dir

= 1.1 =
- add whatsapp|pinterest|linkedin|xing
- include latest upstream changes (fix mail etc.)
- add old default selection of services to make it backward compatible

= 1.0.2 =
- add German translation to the admin menu (Admin-Menue in Deutsch)
- code cleanup

= 1.0.1 =
- add PHP version check (5.4 is needed by the backend option)

= 1.0 =
- add admin menu page
- disable the default add on a post if a special formed tag was found
- add support for the theme attribute

= 0.4 =
- Include latest upstream changes
- use get_permalink() to set the parameter data-url

= 0.3 =
- add support for "hideshariff" 
- add screenshots

= 0.2 =
- removed the private update server and changed test domain 

= 0.1 = 
- initial release
