---
subcategory: "FortiWEB WAF"
layout: "fortiadc"
page_title: "FortiWEB: fortiweb_waf_link_cloaking_link_cloaking_policy"
description: |-
  Configure FortiWEB waf link cloaking link cloaking policy configuration.
---

# fortiweb_waf_link_cloaking_link_cloaking_policy
Configure FortiWEB waf link cloaking link cloaking policy configuration.

## Example Usage
```hcl
resource "fortiweb_waf_link_cloaking_link_cloaking_policy" "test1" {
	mkey = "test"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf link cloaking link cloaking policy entry.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Link Cloaking Link Cloaking Policy can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_link_cloaking_link_cloaking_policy.labelname {mkey}
```
