Cloudera cluster deploy
=========

Creates AWS instances automatically for the cluster and performs initial  configuration of hosts for installing
Cloudera.

Requirements
------------

Boto package is required for the playbook to function

    pip install boto

Also the AWS Access key and Secret key need to be included in the AWS_ACCESS_KEY and AWS_SECRET_KEY environment
variables

Role Variables
--------------

The playbook is mostly automated but there are a few variables that can be set so as to change the default behavior:

* num_slaves - Number of slaves (Default is 3)
* cld_environment - Environment tag in AWS (Default is "Test Environment")
* cld_client - Client tag in AWS (Default is "Atigeo internal")

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Should be launched stand-alone for now.

TO DO

1. Complete automatic add to inventory of new instances
2. Create /etc/hosts file automatically
3. Complete other system init changes
4. Refactor playbook to conform to the folder structure
