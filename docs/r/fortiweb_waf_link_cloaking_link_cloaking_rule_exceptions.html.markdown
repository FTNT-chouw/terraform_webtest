---
subcategory: "FortiWEB WAF"
layout: "fortiadc"
page_title: "FortiWEB: fortiweb_waf_link_cloaking_link_cloaking_rule_exceptions"
description: |-
  Configure FortiWEB waf link cloaking link cloaking rule exceptions configuration.
---

# fortiweb_waf_link_cloaking_link_cloaking_rule_exceptions
Configure FortiWEB waf link cloaking link cloaking rule exceptions configuration.

## Example Usage
```hcl
resource "fortiweb_waf_link_cloaking_link_cloaking_rule_exceptions" "test1" {
	mkey = "test"
	sub_mkey = "1"
	url_type = "plain"
	url_pattern = "/test"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf link cloaking link cloaking rule entry.
* `sub_mkey` - The Id of the waf link cloaking link cloaking rule exceptions entry.
* `url_type` - Select whether the URL Pattern.
* `url_pattern` - The literal URL, such as /folder1/index.htm or regular expression, such as ^/*.php.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Link Cloaking Link Cloaking Rule Exceptions can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_link_cloaking_link_cloaking_rule_exceptions.labelname {mkey}
```
