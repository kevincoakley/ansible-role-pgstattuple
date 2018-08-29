ansible-role-pgstattuple
========================

[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-pgstattuple.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-pgstattuple)

Installs the pgstattuple for PostgreSQL 10 - https://www.postgresql.org/docs/current/static/pgstattuple.html . Tested with pgstattuple 1.5 on CentOS 7.

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml and the example inventory below

Dependencies
------------

None

Example Playbook
----------------

    - name: The pgstattuple role for CentOS
      hosts: pgstattuple
      become: yes
      become_method: sudo
    
      roles:
        - ansible-role-pgstattuple
    
      tags:
        - pgstattuple
    
License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)
