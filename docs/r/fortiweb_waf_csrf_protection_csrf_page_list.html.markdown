---
subcategory: "FortiWEB WAF"
layout: "fortiadc"
page_title: "FortiWEB: fortiweb_waf_csrf_protection_csrf_page_list"
description: |-
  Configure FortiWEB waf csrf protection csrf page list configuration.
---

# fortiweb_waf_csrf_protection_csrf_page_list
Configure FortiWEB waf csrf protection csrf page list configuration.

## Example Usage
```hcl
resource "fortiweb_waf_csrf_protection_csrf_page_list" "test" {
	sub_mkey = "1"
	mkey = "test"
	host_status = "enable"
	host = "test"
	request_type = "plain"
	request_url = "/test"
	parameter_filter = "enable"
	parameter_name = "parameter name"
	parameter_value_type = "plain"
	parameter_value = "parameter value"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf csrf protection entry.
* `sub_mkey` - The id of the waf csrf protection csrf page list entry.
* `host_status` - Enable to apply this rule only to HTTP requests for specific web hosts.
* `host` - Select the name of a protected host.
* `request_type` - Select whether Full URL contains a literal URL, or a regular expression designed to match multiple URLs.
* `request_url` - Enter either a literal URL or regular expression.
* `parameter_filter` - Select to specify a parameter name and value to match.
* `parameter_name` - Enter the parameter name to match.
* `parameter_value_type` - Select whether Parameter Value contains a literal URL or a regular expression designed to match multiple values.
* `parameter_value` - Enter either a literal URL or regular expression.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Csrf Protection Csrf Page List can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_csrf_protection_csrf_page_list.labelname {mkey}
```
