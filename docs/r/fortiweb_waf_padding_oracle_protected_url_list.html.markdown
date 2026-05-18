---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_padding_oracle_protected_url_list"
description: |-
  Configure FortiWEB waf padding oracle protected url list configuration.
---

# fortiweb_waf_padding_oracle_protected_url_list
Configure FortiWEB waf padding oracle protected url list configuration.

## Example Usage
```hcl
resource "fortiweb_waf_padding_oracle_protected_url_list" "test1" {
	mkey = "test"
	sub_mkey = "1"
	host_status = "enable"
	host = "test.com"
	protected_url = "/folder1/*"
	url_type = "plain"
	target = "url parameter"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf padding oracle protected entry.
* `sub_mkey` - The Id of the waf padding oracle protected url list entry.
* `host_status` - Enable to apply this rule only to HTTP requests for specific web hosts. 
* `host` - Select which protected host names entry that the Host of the HTTP request.
* `protected_url` - The literal URL, such as /folder1/index.htm or a regular expression, such as ^/*\.jsp\?uid\=(.*), matching all and only the URLs to which the rule should apply.
* `url_type` - Select whether the Protected URL field must contain a literal URL, or a regular expression designed to match multiple URLs.
* `target` - Indicate which parts of the client’s requests should be examined for padding attack attempts. Valid values: URL, Parameter or Cookie. 

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Padding Oracle Protected Url List can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_padding_oracle_protected_url_list.labelname {mkey}
```
