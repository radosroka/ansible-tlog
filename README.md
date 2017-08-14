ansible-tlog
============

This is ansible tlog role. See https://github.com/Scribery/tlog.

This project is under development.
ReadMe will be updated later.

Requirements
------------

None

Role Variables
--------------

Defaults:
arch: x86_64
source_dir: tlog-source
# could be file/syslog/es
tlog_writer: syslog
tlog_logfile: /var/log/tlog.log
tlog_priority: info
tlog_facility: local5

tlog_reader: file

es_forward: true
# set elasticsearch ip and port
es_ip: 192.168.122.250
es_port: 9200

Dependencies
------------

None

Example Playbook
----------------


    - hosts: all
      roles:
         - { role: username.ansible-galaxy, es_forward: true }

License
-------

GPL3

Author Information
------------------
Radovan Sroka --- rsroka@redhat.com
