---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_certificate_hpkp"
description: |-
  Configure FortiWEB system certificate hpkp configuration.
---

# fortiweb_system_certificate_hpkp
Configure FortiWEB system certificate hpkp configuration.

## Example Usage
```hcl
resource "fortiweb_system_certificate_hpkp" "test" {
	mkey = "test"
	pin_sha256 = "qqq aaa"
	max_age = 1296000
	subdomains = "enable"
	report_only = "enable"
	report_uri = "aaa.com"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system certificate hpkp entry.
* `pin_sha256` - Pin-Sha256 setting.
* `max_age` - Max-Age setting.
* `subdomains` - Subdomains setting.
* `report_uri` - Report-Uri setting.
* `report_only` - Report-Only setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Certificate Hpkp can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_certificate_hpkp.labelname {mkey}
```
