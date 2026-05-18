---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_link_cloaking_link_cloaking_policy_rule_list"
description: |-
  Configure FortiWEB waf link cloaking link cloaking policy rule list configuration.
---

# fortiweb_waf_link_cloaking_link_cloaking_policy_rule_list
Configure FortiWEB waf link cloaking link cloaking policy rule list configuration.

## Example Usage
```hcl
resource "fortiweb_waf_link_cloaking_link_cloaking_policy_rule_list" "test1" {
	mkey = "test"
	sub_mkey = "1"
	rule = "test"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf link cloaking link cloaking policy entry.
* `sub_mkey` - The Id of the waf link cloaking link cloaking policy rule list entry.
* `rule` - Select the name of waf link cloaking link cloaking rule.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Link Cloaking Link Cloaking Policy Rule List can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_link_cloaking_link_cloaking_policy_rule_list.labelname {mkey}
```
