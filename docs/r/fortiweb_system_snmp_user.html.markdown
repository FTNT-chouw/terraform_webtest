---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_snmp_user"
description: |-
  Configure FortiWEB system snmp user configuration.
---

# fortiweb_system_snmp_user
Configure FortiWEB system snmp user configuration.

## Example Usage
```hcl
resource "fortiweb_system_snmp_user" "test" {
	mkey = "test"
	status = "enable"
	security_level = "authpriv"
	auth_proto = "sha1"
	auth_pwd = "fortinet"
	priv_proto = "aes"
	priv_pwd = "fortinet"
	query_status = "enable"
	query_port = 161
	trap_status = "enable"
	trapport_local = 163
	trapport_remote = 164
	trapevent = "cpu-high mem-low log-full sys-mode-change intf-ip sys-ha-cluster-status-change sys-ha-member-join sys-ha-member-leave policy-start policy-stop pserver-failed waf-amethod-attack waf-pvalid-attack waf-hidden-fields waf-url-access-attack waf-signature-detection netlink-up-status netlink-down-status power-supply-failure policy-ldap-auth-failure policy-radius-auth-failure"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system snmp user entry.
* `status` - Enable to activate the community.
* `security_level` - Security-Level setting.
* `auth_proto` - Auth-Proto setting.
* `auth_pwd` - Auth-Pwd setting.
* `priv_proto` - Priv-Proto setting.
* `priv_pwd` - Priv-Pwd setting.
* `query_status` - Query-Status setting.
* `query_port` - Query-Port setting.
* `trap_status` - Trap-Status setting.
* `trapport_local` - Trapport-Local setting.
* `trapport_remote` - Trapport-Remote setting.
* `trapevent` - Trapevent setting.
* `ip` - Ip setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Snmp User can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_snmp_user.labelname {mkey}
```
