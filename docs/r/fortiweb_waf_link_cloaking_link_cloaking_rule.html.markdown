---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_link_cloaking_link_cloaking_rule"
description: |-
  Configure FortiWEB waf link cloaking link cloaking rule configuration.
---

# fortiweb_waf_link_cloaking_link_cloaking_rule
Configure FortiWEB waf link cloaking link cloaking rule configuration.

## Example Usage
```hcl
resource "fortiweb_waf_link_cloaking_link_cloaking_rule" "test1" {
	mkey = "test"
	host_status = "enable"
	host = "tesa"
	url_type = "plain"
	url_pattern = "/test"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf link cloaking link cloaking rule entry.
* `host_status` - Enable to require that the Host of the HTTP request matches a protected host name entry in order to match the link cloaking rule.
* `host` - Select the protected host names entry.
* `url_type` - Select whether the URL Pattern.
* `url_pattern` - The literal URL, such as /folder1/index.htm or regular expression, such as ^/*.php.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Link Cloaking Link Cloaking Rule can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_link_cloaking_link_cloaking_rule.labelname {mkey}
```
