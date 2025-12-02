---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_certificate_letsencrypt"
description: |-
  Configure FortiWEB system certificate letsencrypt configuration.
---

# fortiweb_system_certificate_letsencrypt
Configure FortiWEB system certificate letsencrypt configuration.

## Example Usage
```hcl
resource "fortiweb_system_certificate_letsencrypt" "test" {
	mkey = "testlets"
	domain = "1.1.1.1"
	validation_method = "HTTP-01"
	key_type = "RSA-2048"
	renew_period = 30
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system certificate letsencrypt entry.
* `domain` - Domain setting.
* `status` - Status setting.
* `validation_method` - Validation-Method setting.
* `key_type` - Key-Type setting.
* `retry_times` - Retry-Times setting.
* `acme_service` - Acme-Service setting.
* `acme_service_url` - Acme-Service-Url setting.
* `acme_eab` - Acme-Eab setting.
* `eab` - Eab setting.
* `acme_email` - Acme-Email setting.
* `expire_date` - Expire-Date setting.
* `certificate` - Certificate setting.
* `private_key` - Private-Key setting.
* `tls_validation_certificate` - Tls-Validation-Certificate setting.
* `tls_validation_private_key` - Tls-Validation-Private-Key setting.
* `renew_period` - Renew-Period setting.
* `type` - Type setting.
* `san_dns` - San-Dns setting.
* `san_ip` - San-Ip setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Certificate Letsencrypt can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_certificate_letsencrypt.labelname {mkey}
```
