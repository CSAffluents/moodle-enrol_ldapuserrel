This plugin allows you to configure automatic relationships between users from LDAP

THIS PLUGIN HAS BEEN USED FOR MORE THAN A YEAR BUT BE CAREFULL WITH PRODUCTION ENVIRONMENT!

Users familiar with enrol/ldap should have no problems configuring this.

Plugin has been tested on 2.6.1.

This plugin is the LDAP version of a plugin that was first developed by Penny Leach <penny@catalyst.net.nz> for Moodle 1.9
but I modified it to work with Moodle 2.3

This is one of my first experience with Moodle plugin development, so your comments are more than
welcome. Useless to say that you use this piece of code at your own risk :)

HOW TO INSTALL
==============
Prerequisis
a. LDAP server with mentor entries with an attribute containing a list of mentee id
b. PHP library to connect to LDAP
c. mentee and mentor accounts already in Moodle

1. Download all the files in the directory {MOODLE_DIR}/enrol/ldapuserrel (using git, GitHub website, or anything else)
2. Go to http://{MOODLE_URL}/admin to complete the installation
3. Fill all parameters using Moodle plugin administration interface (http://{MOODLE_URL}/admin/settings.php?section=enrolsettingsldapuserrel)
4. Setup a cron job to execute {MOODLE_DIR}/enrol/ldapuserrel/cli/sync.php (add -v for more output, and redirecte output to log file)

Feel free to send me any comments/suggestions

Maxime Pelletier <maxime.pelletier@educsa.org>
