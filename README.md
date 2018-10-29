# 2xx
For WEB 230 - Web Databases
php/mysql steps to the inside-out-project

https://2xx.donaldallenjr.com

Version 200.0

	- pulled files from clients HTML site and uploaded to the development server.
	- updated title tag and header title with PHP variable.
	- converted all HTML comments to PHP comments.

Version 201.0

	- replaced top level pages by changing them to php files. (love, who, challenges, you)
	- removed header and footer from the pages replaced.
	- ctreated the include folders
	- created the header.inc.php and footer.inc.php files.

Version 202.0

	- replaced navigation menu with top level pages by creating a function and array to dynamically create the menu (love, who, challenges, you)
	- created the functions.inc.php file
		- created the menuBuilder function
	- created the menu.data.php file
		- created menuItems array
	- included in the very top of the header.inc.php a require_once to the include/menu.data.php file
	- included in the very top of the header.inc.php a require_once to the include/functions.inc.php file

Version 203.0

	- rename the menu.data.php page to content.data.php and made updates in header.inc.php
		- make modifications to the content.data.php page
			- change the variable/array name from "$menuItems" to "$content"
			- replace all instances of "MenuLink" with "pageLink"
			- replace all instances of "MenuName" with "pageName"
			- add the "childPages" sub-array for each of the pages
		- updated the menuBuilder() function to recursivly handle child data
		- created a config.inc.php file to keep our global variables in as we create them.
		- added the code to the footer.inc.php page to add the copyright and version information.
		- added class to the style.css page for the copyright and version. (.copyright)
		- added redirect to force a secure connection in the header.inc.php.
