Role Name
=========

Takes a list of 1. Repos 2. Addons to the end of the repo 3. Package names to download from the repo, and installs them

Requirements
------------

NA

Role Variables
--------------

my_pkgs - Overall containing for all the packages to be downloaded. Each package within my_pkg requires a standard layout for the package_installer to correctly parse them;

my_pkgs:
    - <name of sub-group>
    repo: <repo base url>
    add: <any part of the url beyond .com/>
    name: <name of package>
    
Subgroups can be repeated infinitely

Dependencies
------------

NA

Example Playbook
----------------

I dont actually know how to do variables in a playbook yet lel.

    - hosts: all
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD
