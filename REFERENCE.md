# Reference
<!-- DO NOT EDIT: This document was generated by Puppet Strings -->

## Table of Contents

**Classes**

_Public Classes_

* [`epel`](#epel): Configure the proper EPEL repositories and import GPG keys

_Private Classes_

* `epel::params`: 

**Defined types**

_Public Defined types_


_Private Defined types_

* `epel::rpm_gpg_key`: Import an RPM gpg key

## Classes

### epel

Configure the proper EPEL repositories and import GPG keys

* **See also**
https://fedoraproject.org/wiki/EPEL

#### Examples

##### Basic Usage

```puppet
include epel
```

#### Parameters

The following parameters are available in the `epel` class.

##### `epel_managed`

Data type: `Boolean`

Determines if the main EPEL repository is managed.

Default value: `true`

##### `epel_source_managed`

Data type: `Boolean`

Determines if the `epel-source` repository is managed.

Default value: `true`

##### `epel_debuginfo_managed`

Data type: `Boolean`

Determines if the `epel-debuginfo` repository is managed.

Default value: `true`

##### `epel_testing_managed`

Data type: `Boolean`

Determines if the `epel-testing` repository is managed.

Default value: `true`

##### `epel_testing_source_managed`

Data type: `Boolean`

Determines if the `epel-testing-source` repository is managed.

Default value: `true`

##### `epel_testing_debuginfo_managed`

Data type: `Boolean`

Determines if the `epel-testing-debuginfo` repository is managed.

Default value: `true`

##### `epel_gpg_managed`

Data type: `Boolean`

Detemines if the module manages the rpm-gpg key for EPEL.

Default value: `true`

##### `epel_mirrorlist`

Data type: `Any`



Default value: $epel::params::epel_mirrorlist

##### `epel_baseurl`

Data type: `Any`



Default value: $epel::params::epel_baseurl

##### `epel_failovermethod`

Data type: `Any`



Default value: $epel::params::epel_failovermethod

##### `epel_proxy`

Data type: `Any`



Default value: $epel::params::epel_proxy

##### `epel_enabled`

Data type: `Any`



Default value: $epel::params::epel_enabled

##### `epel_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_gpgcheck

##### `epel_repo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_repo_gpgcheck

##### `epel_metalink`

Data type: `Any`



Default value: $epel::params::epel_metalink

##### `epel_exclude`

Data type: `Any`



Default value: `undef`

##### `epel_includepkgs`

Data type: `Any`



Default value: `undef`

##### `epel_sslclientkey`

Data type: `Any`



Default value: `undef`

##### `epel_sslclientcert`

Data type: `Any`



Default value: `undef`

##### `epel_testing_mirrorlist`

Data type: `Any`



Default value: $epel::params::epel_testing_mirrorlist

##### `epel_testing_baseurl`

Data type: `Any`



Default value: $epel::params::epel_testing_baseurl

##### `epel_testing_failovermethod`

Data type: `Any`



Default value: $epel::params::epel_testing_failovermethod

##### `epel_testing_proxy`

Data type: `Any`



Default value: $epel::params::epel_testing_proxy

##### `epel_testing_enabled`

Data type: `Any`



Default value: $epel::params::epel_testing_enabled

##### `epel_testing_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_testing_gpgcheck

##### `epel_testing_repo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_testing_repo_gpgcheck

##### `epel_testing_metalink`

Data type: `Any`



Default value: $epel::params::epel_testing_metalink

##### `epel_testing_exclude`

Data type: `Any`



Default value: `undef`

##### `epel_testing_includepkgs`

Data type: `Any`



Default value: `undef`

##### `epel_testing_sslclientkey`

Data type: `Any`



Default value: `undef`

##### `epel_testing_sslclientcert`

Data type: `Any`



Default value: `undef`

##### `epel_source_mirrorlist`

Data type: `Any`



Default value: $epel::params::epel_source_mirrorlist

##### `epel_source_baseurl`

Data type: `Any`



Default value: $epel::params::epel_source_baseurl

##### `epel_source_failovermethod`

Data type: `Any`



Default value: $epel::params::epel_source_failovermethod

##### `epel_source_proxy`

Data type: `Any`



Default value: $epel::params::epel_source_proxy

##### `epel_source_enabled`

Data type: `Any`



Default value: $epel::params::epel_source_enabled

##### `epel_source_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_source_gpgcheck

##### `epel_source_repo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_source_repo_gpgcheck

##### `epel_source_metalink`

Data type: `Any`



Default value: $epel::params::epel_source_metalink

##### `epel_source_exclude`

Data type: `Any`



Default value: `undef`

##### `epel_source_includepkgs`

Data type: `Any`



Default value: `undef`

##### `epel_source_sslclientkey`

Data type: `Any`



Default value: `undef`

##### `epel_source_sslclientcert`

Data type: `Any`



Default value: `undef`

##### `epel_debuginfo_mirrorlist`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_mirrorlist

##### `epel_debuginfo_baseurl`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_baseurl

##### `epel_debuginfo_failovermethod`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_failovermethod

##### `epel_debuginfo_proxy`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_proxy

##### `epel_debuginfo_enabled`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_enabled

##### `epel_debuginfo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_gpgcheck

##### `epel_debuginfo_repo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_repo_gpgcheck

##### `epel_debuginfo_metalink`

Data type: `Any`



Default value: $epel::params::epel_debuginfo_metalink

##### `epel_debuginfo_exclude`

Data type: `Any`



Default value: `undef`

##### `epel_debuginfo_includepkgs`

Data type: `Any`



Default value: `undef`

##### `epel_debuginfo_sslclientkey`

Data type: `Any`



Default value: `undef`

##### `epel_debuginfo_sslclientcert`

Data type: `Any`



Default value: `undef`

##### `epel_testing_source_mirrorlist`

Data type: `Any`



Default value: $epel::params::epel_testing_source_mirrorlist

##### `epel_testing_source_baseurl`

Data type: `Any`



Default value: $epel::params::epel_testing_source_baseurl

##### `epel_testing_source_failovermethod`

Data type: `Any`



Default value: $epel::params::epel_testing_source_failovermethod

##### `epel_testing_source_proxy`

Data type: `Any`



Default value: $epel::params::epel_testing_source_proxy

##### `epel_testing_source_enabled`

Data type: `Any`



Default value: $epel::params::epel_testing_source_enabled

##### `epel_testing_source_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_testing_source_gpgcheck

##### `epel_testing_source_repo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_testing_source_repo_gpgcheck

##### `epel_testing_source_metalink`

Data type: `Any`



Default value: $epel::params::epel_testing_source_metalink

##### `epel_testing_source_exclude`

Data type: `Any`



Default value: `undef`

##### `epel_testing_source_includepkgs`

Data type: `Any`



Default value: `undef`

##### `epel_testing_source_sslclientkey`

Data type: `Any`



Default value: `undef`

##### `epel_testing_source_sslclientcert`

Data type: `Any`



Default value: `undef`

##### `epel_testing_debuginfo_mirrorlist`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_mirrorlist

##### `epel_testing_debuginfo_baseurl`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_baseurl

##### `epel_testing_debuginfo_failovermethod`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_failovermethod

##### `epel_testing_debuginfo_proxy`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_proxy

##### `epel_testing_debuginfo_enabled`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_enabled

##### `epel_testing_debuginfo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_gpgcheck

##### `epel_testing_debuginfo_repo_gpgcheck`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_repo_gpgcheck

##### `epel_testing_debuginfo_metalink`

Data type: `Any`



Default value: $epel::params::epel_testing_debuginfo_metalink

##### `epel_testing_debuginfo_exclude`

Data type: `Any`



Default value: `undef`

##### `epel_testing_debuginfo_includepkgs`

Data type: `Any`



Default value: `undef`

##### `epel_testing_debuginfo_sslclientkey`

Data type: `Any`



Default value: `undef`

##### `epel_testing_debuginfo_sslclientcert`

Data type: `Any`



Default value: `undef`

##### `os_maj_release`

Data type: `Any`



Default value: $epel::params::os_maj_release

## Defined types

