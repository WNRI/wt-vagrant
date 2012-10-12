Vagrant package for Waymarked Trails

This is the repository for the vagrant package for Waymarked Trails. Please see [Testing with vagrant](https://github.com/lonvia/waymarked-trails-site/wiki/Testing-with-vagrant) and [Making a vagrant box](https://github.com/WNRI/route.is/wiki/Making-a-vagrant-box) for more information about the use and making of the box.

This repository includes files used to make the box, including the Vagrantfile.

## Contents

`apache`: Virtual host configurations for apache. Belongs in `/etc/apache2/sites-available/`

`Vagrantfile`: Symbolic link to `Vagrantfile.pkg` to facilitate easy use of repository as box directory.

`cookbooks`: Directory for cookbooks that can be used for provisioning with chef. No provisioning is used at the moment however.

`post-receive`: Post-receive hook for bare git repository to set up web serving directory and restart web server.

`settings_local.py`: Local settings needed to serve from localhost. Belongs in `/srv/www/wt-test/django/src/routemap/common/`

`Vagrantfile.pkg`: The vagrant configuration used to set up the box.

## Copyright

See LICENSE
