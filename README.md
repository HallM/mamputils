# mamputils
For those who don't want to deal with vhosts (like dev machines)

Some utilities for managing mamp with a sites-available/-enabled

Sets up Alias and basic Directory conf for a project in a sub directory

# Requirements & Set up
Written for mamp, though doesn't rely on mamp necessarily. Just requires Apache

All scripts must be in a directory with the same parent directory as apache2
Ex:
- /path/to/apache2
- /path/to/mamputils

The folders 'subdir-available' and 'subdir-enabled' must be created within apache's directory

Add the following to the end of the httpd.conf file:
```
IncludeOptional "subdir-enabled/*.conf"
```
