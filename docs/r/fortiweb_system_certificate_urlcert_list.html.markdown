---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_certificate_urlcert_list"
description: |-
  Configure FortiWEB system certificate urlcert list configuration.
---

# fortiweb_system_certificate_urlcert_list
Configure FortiWEB system certificate urlcert list configuration.

## Example Usage
```hcl
resource "fortiweb_system_certificate_urlcert_list" "test" {
	mkey = "test"
	sub_mkey = "1"
	url = "1.1.1.1"
	require = "enable"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system certificate urlcert list entry.
* `id` - Id setting.
* `url` - Url setting.
* `require` - Require setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Certificate Urlcert List can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_certificate_urlcert_list.labelname {mkey}
```
