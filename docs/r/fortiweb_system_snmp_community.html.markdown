---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_snmp_community"
description: |-
  Configure FortiWEB system snmp community configuration.
---

# fortiweb_system_snmp_community
Configure FortiWEB system snmp community configuration.

## Example Usage
```hcl
resource "fortiweb_system_snmp_community" "test" {
	mkey = "1"
	name = "test"
	status = "enable"
	query_v1_status = "enable"
	query_v1_port = 161
	query_v2c_status = "enable"
	query_v2c_port = 162
	trap_v1_status = "enable"
	trap_v1_lport = 163
	trap_v1_rport = 164
	trap_v2c_status = "enable"
	trap_v2c_lport = 165
	trap_v2c_rport = 166
	events = "cpu-high mem-low log-full sys-mode-change intf-ip sys-ha-cluster-status-change sys-ha-member-join sys-ha-member-leave policy-start policy-stop pserver-failed waf-amethod-attack waf-pvalid-attack waf-hidden-fields waf-url-access-attack waf-signature-detection netlink-up-status netlink-down-status power-supply-failure policy-ldap-auth-failure policy-radius-auth-failure"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system snmp community entry.
* `name` - Name setting.
* `status` - Status setting.
* `ip` - Ip setting.
* `query_v1_status` - Query-V1-Status setting.
* `query_v1_port` - Query-V1-Port setting.
* `query_v2c_status` - Query-V2C-Status setting.
* `query_v2c_port` - Query-V2C-Port setting.
* `trap_v1_status` - Trap-V1-Status setting.
* `trap_v1_lport` - Trap-V1-Lport setting.
* `trap_v1_rport` - Trap-V1-Rport setting.
* `trap_v2c_status` - Trap-V2C-Status setting.
* `trap_v2c_lport` - Trap-V2C-Lport setting.
* `trap_v2c_rport` - Trap-V2C-Rport setting.
* `events` - Events setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Snmp Community can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_snmp_community.labelname {mkey}
```
