---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_http_header_security_http_header_security_list"
description: |-
  Configure FortiWEB waf http header security http header security list configuration.
---

# fortiweb_waf_http_header_security_http_header_security_list
Configure FortiWEB waf http header security http header security list configuration.

## Example Usage
```hcl
resource "fortiweb_waf_http_header_security_http_header_security_list" "test" {
	mkey = "test"
	sub_mkey = "1"
	exception = "test"
	request_file = "/test.htm"
	request_status = "enable"
	request_type = "plain"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf http header security.
* `sub_mkey` - The id of the waf http header security http header security list entry.
* `exception` - The name of a new or existing HTTP protocol constraint exception.
* `request_file` - Sets the Request URL for the URL Filter.
* `request_status` - Enable to set a URL Filter.
* `request_type` - Defines the Request URL Type as a simple string (plain) or a regular expression (regular) for the URL Filter.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Http Header Security Http Header Security List can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_http_header_security_http_header_security_list.labelname {mkey}
```
