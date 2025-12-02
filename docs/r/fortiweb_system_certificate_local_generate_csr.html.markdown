---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_certificate_local_generate_csr"
description: |-
  Configure FortiWEB system certificate local generate csr configuration.
---

# fortiweb_system_certificate_local_generate_csr
Configure FortiWEB system certificate local generate csr configuration.

## Example Usage
```hcl
resource "fortiweb_system_certificate_local_generate_csr" "test" {
	mkey = "test"
	idtype = "hostIp"
	ip = "0.0.0.0"
	organizationunit_1 = "orgunit"
	organization = "org"
	localitycity = "city1"
	stateprovince = "state1"
	countryregion = "US"
	email = "test@test.com"
	subject_alternative_type_1 = "domainname"
	subject_alternative_text_1 = "aaaa.com"
	keysize = "2048"
	digestalgorithm = "SHA256"
	enrollmentmethod = "file"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system certificate local entry.
* `type` - Type setting.
* `status` - Status setting.
* `comment` - Comment setting.
* `flag` - Flag setting.
* `is_hsm` - Is-Hsm setting.
* `partition_number` - Partition-Number setting.
* `certificate` - Certificate setting.
* `private_key` - Private-Key setting.
* `passwd` - Passwd setting.
* `is_primus_hsm` - Is-Primus-Hsm setting.
* `primus_partition` - Primus-Partition setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Certificate Local can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_certificate_local_generate_csr.labelname {mkey}
```
