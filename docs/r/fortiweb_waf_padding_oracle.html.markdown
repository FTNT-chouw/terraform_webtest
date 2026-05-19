---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_padding_oracle"
description: |-
  Configure FortiWEB waf padding oracle configuration.
---

# fortiweb_waf_padding_oracle
Configure FortiWEB waf padding oracle configuration.

## Example Usage
```hcl
resource "fortiweb_waf_padding_oracle" "test" {
	mkey = "test"
	action = "alert"
	block_period = 600
	severity = "Medium"
	trigger = "test"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf padding oracle entry.
* `action` -  Select which action the FortiWeb appliance will take when it detects a violation of the rule. Valid values: Alert, Alert & Deny, Deny, Period Block.
* `block_period` - Type the number of seconds that you want to block subsequent requests from the client after the FortiWeb appliance detects that the client has violated the rule. Valid values: 1-3600.
* `severity` - Select which severity level the FortiWeb appliance will use when it logs a violation of the rule. Valid values: Informative, Low, Medium, High.
* `trigger` - Select the trigger.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Padding Oracle can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_padding_oracle.labelname {mkey}
```
