ansible-tlog
============

This is ansible tlog role. See https://github.com/Scribery/tlog.

This project is under development.

Requirements
------------

None

Role Variables
--------------

Defaults:  
* arch: x86_64  
* source_dir: tlog-source  
* tlog_writer: syslog (could be file/syslog/es)  
* tlog_logfile: /var/log/tlog.log  
* tlog_priority: info  
* tlog_facility: local5

* tlog_reader: file  

* es_forward: false  

#set elasticsearch ip and port
* es_ip: 127.0.0.1  
* es_port: 9200  

Dependencies
------------

None

Example Playbook
----------------


    - hosts: all
      roles:
         - { role: radosroka.ansible-tlog }

License
-------

GPL3

Author Information
------------------
Radovan Sroka --- rsroka@redhat.com
