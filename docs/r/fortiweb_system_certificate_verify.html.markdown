---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_certificate_verify"
description: |-
  Configure FortiWEB system certificate verify configuration.
---

# fortiweb_system_certificate_verify
Configure FortiWEB system certificate verify configuration.

## Example Usage
```hcl
resource "fortiweb_system_certificate_verify" "test" {
	mkey = "testcertverify"
	ca = "test"
	crl = "test"
	ocsp = "testocsprep"
	publish_dn = "enable"
	strictly_need_cert = "disable"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system certificate verify entry.
* `ca` - Ca setting.
* `crl` - Crl setting.
* `ocsp` - Ocsp setting.
* `publish_dn` - Publish-Dn setting.
* `strictly_need_cert` - Strictly-Need-Cert setting.
* `partial_chain` - Partial-Chain setting.
* `crl_allow_expired` - Crl-Allow-Expired setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Certificate Verify can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_certificate_verify.labelname {mkey}
```
