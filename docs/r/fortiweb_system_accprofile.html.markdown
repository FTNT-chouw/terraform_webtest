---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_accprofile"
description: |-
  Configure FortiWEB system accprofile configuration.
---

# fortiweb_system_accprofile
Configure FortiWEB system accprofile configuration.

## Example Usage
```hcl
resource "fortiweb_system_accprofile" "test" {
	mkey = "test"
	mntgrp = "rw"
	admingrp = "rw"
	sysgrp = "none"
	netgrp = "none"
	loggrp = "r"
	authusergrp = "r"
	traroutegrp = "rw"
	wafgrp = "rw"
	wadgrp = "none"
	wvsgrp = "none"
	mlgrp = "r"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system accprofile entry.
* `mntgrp` - Mntgrp setting.
* `admingrp` - Admingrp setting.
* `sysgrp` - Sysgrp setting.
* `netgrp` - Netgrp setting.
* `loggrp` - Loggrp setting.
* `authusergrp` - Authusergrp setting.
* `traroutegrp` - Traroutegrp setting.
* `wafgrp` - Wafgrp setting.
* `wadgrp` - Wadgrp setting.
* `wvsgrp` - Wvsgrp setting.
* `mlgrp` - Mlgrp setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Accprofile can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_accprofile.labelname {mkey}
```
