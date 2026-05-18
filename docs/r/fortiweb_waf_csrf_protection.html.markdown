---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_csrf_protection"
description: |-
  Configure FortiWEB waf csrf protection configuration.
---

# fortiweb_waf_csrf_protection
Configure FortiWEB waf csrf protection configuration.

## Example Usage
```hcl
resource "fortiweb_waf_csrf_protection" "test" {
	mkey = "test"
	action = "alert"
	block_period = 600
	severity = "Low"
	trigger = "test"
	js_request_check = "enable"
}
```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf csrf protection entry.
* `action` - Select which action FortiWeb takes when it detects a missing or incorrect anti-CSRF parameter. Valid values: Alert, Alert & Deny, Deny, Period Block.
* `block_period` - Enter the number of seconds that you want to block subsequent requests from the client after the FortiWeb appliance detects a CSRF attack.  Valid values: 1-3600.
* `severity` - Select which severity level FortiWeb uses when it logs a CSRF attack. Valid values: Informative, Low, Medium, High. 
* `trigger` - Select the trigger.
* `js_request_check` - By default, FortiWeb runs a script to append the parameter tknfv (the anti-CSRF token) to any HTML link elements. 

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Csrf Protection can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_csrf_protection.labelname {mkey}
```
