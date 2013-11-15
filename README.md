chef-fatclient-builder
======================

Creates a Joyent Operations-style Chef Fatclient for use on SmartOS which is used by
the Cloud Operations guys at Siberia and TextDrive.  Ben Rockwood does not endorse
the usage of this script.  It was created outside of Joyent by Jacques Marneweck as
I was a frequent user of the Joyent Operations-style Chef Fatclient while on the
Operations Team at Joyent.  I continue to use the Joyent Operations-style Chef
Fatclient on a daily basis.  This script builds a version of Ruby 1.9.3 and with the
latest version of Chef and Ohai.

Process
-------

It is best to delete /opt/chef before starting.  Then run the build-fatclient-bundle
script.  The tarball created during the process can be found under /var/tmp

Known Bugs
----------

 * You have to install libyaml from pkgsrc at present as ruby ignores the custom compiled
   version of libyaml.

Authors
-------

 * Jacques Marneweck (jacques@powertrip.co.za)
