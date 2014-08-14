# puppet-module-vmware
===

[![Build Status](https://travis-ci.org/emahags/puppet-module-vmware.png?branch=master)](https://travis-ci.org/emahags/puppet-module-vmware)

Manage VMware - Install vmwaretools. Will remove vmware tools that has been installed from script if present.

===

# Class `vmware`

## Parameters

manage_repo_package
-------------------
Should repo package be managed? Contains the vmware repo and key.

- *Default*: true

repo_package_name
-----------------
Name of repo package. Please note that this needs to be built manually, there is no premade package.

- *Default*: 'vmwaretools-repo'

repo_package_ensure
-------------------
String to pass to ensure attribute for the repo package.

- *Default*: 'present'

manage_tools_package
--------------------
Should vmwaretools package be managed?

- *Default*: true

tools_package_name
------------------
Name of package(s) for vmwaretools.

- *Default*: based on if X is installed or not.

tools_package_ensure
--------------------
String to pass to ensure attribute for the vmwaretools package.

- *Default*: 'present'
