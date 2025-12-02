---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_certificate_server_certificate_verify"
description: |-
  Configure FortiWEB system certificate server certificate verify configuration.
---

# fortiweb_system_certificate_server_certificate_verify
Configure FortiWEB system certificate server certificate verify configuration.

## Example Usage
```hcl
resource "fortiweb_system_certificate_server_certificate_verify" "test" {
	mkey = "testservercertverify"
	ca = "test"
	crl = "test"
	ocsp = "testocsprep"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system certificate server certificate verify entry.
* `ca` - Ca setting.
* `crl` - Crl setting.
* `ocsp` - Ocsp setting.
* `crl_allow_failure` - Crl-Allow-Failure setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Certificate Server Certificate Verify can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_certificate_server_certificate_verify.labelname {mkey}
```
