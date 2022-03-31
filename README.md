netdata-agent
=========

Install and configure a netdata monitoring agent

Requirements
------------

None.

Role Variables
--------------

**General variables**
- `systemd_unit_name`: name of the systemd service, defaults to `netdata.service`
- `use_stable_packages`: whether to use stable packages or nightly packages (defaults to using stable packages)

**Sending metrics to another instance**
- `send_stream`: whether to enable sending metrics to another server (default: `off`)
- `api_key`: The api key to use for sending metrics, uses a dummy entry as default (`4298d07f-abf7-439f-8a2a-a29e8c9525fa`)   

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
