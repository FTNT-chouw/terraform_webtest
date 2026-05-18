---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_custom_access_policy_rule"
description: |-
  Configure FortiWEB waf custom access policy rule configuration.
---

# fortiweb_waf_custom_access_policy_rule
Configure FortiWEB waf custom access policy rule configuration.

## Example Usage
```hcl
resource "fortiweb_waf_custom_access_policy_rule" "test1" {
	mkey = "test"
	sub_mkey = "1"
	rule_name = "Brute-Force-Login"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf custom access policy entry.
* `sub_mkey` - The ID of the waf custom access policy rule entry.
* `rule_name` - Select the custom rule. Valid values: Brute-Force-Login, Vulnerability-Scanning, Content-Encoding-Evasion, Brute-Force-Login - Alert Only, Vulnerability-Scanning - Alert Only or Content-Encoding-Evasion - Alert Only.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Custom Access Policy Rule can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_custom_access_policy_rule.labelname {mkey}
```
