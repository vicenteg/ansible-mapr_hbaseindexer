mapr_hbaseindexer
=========

Ansible role to install and configure the HBase Indexer 1.5.1.

Requirements
------------

A MapR cluster with Apache HBase installed.

Role Variables
--------------

	hbase_version: 0.98.7
	java_home: /etc/alternatives/java_sdk
	solr_version: 4.10.3
	solr_collection: collection1
	indexer_name: product_indexer
	proxy_env: {}

Dependencies
------------

Example Playbook
----------------

	- hosts: regionserver
	  vars_files:
	    - vars/global/main.yml
	  roles:
	    - { role: mapr_hbaseindexer }

License
-------

MIT

Author Information
------------------

Vince Gonzalez
