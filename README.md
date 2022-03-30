netdata-agent
=========

Install and configure a netdata monitoring agent

Requirements
------------

None.

Role Variables
--------------

- `systemd_unit_name`: name of the systemd service, defaults to `netdata.service`
- `use_stable_packages`: whether to use stable packages or nightly packages (defaults to using stable packages)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: 'johanneskastl.netdata-agent' }

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
