Showcase
=========

[![Build Status](https://ci.corchestra.ru/buildStatus/icon?job=tomcatansible/master)](https://ci.corchestra.ru/job/showcaseansible/job/master/)

Installation of [Showcase](https://corchestra.ru/wiki/index.php?title=Showcase) platform in Tomcat. This role should be run after [CourseOrchestra.tomcat](https://galaxy.ansible.com/CourseOrchestra/tomcat/).

Requirements
------------

* Java 8
* Tomcat (provided by [CourseOrchestra.tomcat](https://galaxy.ansible.com/CourseOrchestra/tomcat/) role)


Role Variables
--------------

* showcase_build: Showcase build number

Example Playbook
----------------

    - hosts: servers
      vars:
         oracle_java_version: 8
         oracle_java_version_update: 131
      roles:
         - role: ansiblebit.oracle-java
         - role: CourseOrchestra.tomcat
         - role: CourseOrchestra.showcase

License
-------

MIT

Author Information
------------------

https://corchestra.ru/en
