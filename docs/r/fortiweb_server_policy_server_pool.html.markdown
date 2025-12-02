---
subcategory: "FortiWEB Server Policy"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_server_policy_server_pool"
description: |-
  Configure FortiWEB server policy server pool configuration.
---

# fortiweb_server_policy_server_pool
Configure FortiWEB server policy server pool configuration.

## Example Usage
```hcl
resource "fortiweb_server_policy_server_pool" "test" {
	mkey = "sp3"
	type = "reverse-proxy"
	server_balance = "disable"
	comment = "test"
	health = "HLTHCK_TCP"
	hlck_sip = "0.0.0.0/0"
	hlck_sip6 = "::/0"
	lb_algo = "round-robin"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The Name of the server policy server pool entry.
* `type` - Type setting. Default is reverse-proxy.
* `protocol` - Specific options for a server pool become available. Default is HTTP.
* `server_balance` - Specifies whether the pool contains a single server or multiple members. Valid values: enable or disable.
* `health` - The name of a server health check FortiWeb uses to determine the responsiveness of server pool members.
* `hlck_sip` - The IP address of Hlck-Sip setting.
* `hlck_sip6` - The IPv6 address of Hlck-Sip6 setting.
* `lb_algo` - Select the load-balancing algorithms that FortiWeb uses when it distributes new connections among server pool members.
* `comment` - Enter a description or other comment.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Server Policy Server Pool can be imported using any of these accepted formats:
```
$ terraform import fortiweb_server_policy_server_pool.labelname {mkey}
```
