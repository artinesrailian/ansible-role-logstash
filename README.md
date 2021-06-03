Ansible Role: Logstash
=========

This role is compatible with RedHat/CentOS 7 and Ubuntu 18.04

Role Variables
--------------

  java_ubuntu: openjdk-11-jdk

The Java version to be installed on Ubuntu

  java_redhat: java-1.8.0-openjdk

The Java version to be installed on CentOS/RedHat

  logstash_version: '7.x'

The major version of the Logstash to be installed

  logstash_listen_port_beats: 5044

The port which Logstash will listen for beats

  logstash_local_syslog_path: /var/log/syslog

The local syslog file path

  logstash_elasticsearch_host: http://localhost:9202

The Elasticsearch host address where Logstash will send the logs

Example Playbook
----------------

    - hosts: servers
      roles:
         - artinesrailian.logstash

License
-------

BSD

Author Information
------------------

The role was created in 2021 by [Artin Esrailian](https://github.com/artinesrailian/).
