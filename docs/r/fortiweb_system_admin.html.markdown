---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_admin"
description: |-
  Configure FortiWEB system admin configuration.
---

# fortiweb_system_admin
Configure FortiWEB system admin configuration.

## Example Usage
```hcl
resource "fortiweb_system_admin" "test" {
	mkey = "test"
	type = "local-user"
	trusthostv4 = "0.0.0.0/0 "
	trusthostv6 = "::/0 "
	access_profile = "admin_no_access"
	force_password_change = "disable"
	password = "test"
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system admin entry.
* `access_profile` - Access-Profile setting.
* `trusthostv4` - Trusthostv4 setting.
* `trusthostv6` - Trusthostv6 setting.
* `last_name` - Last-Name setting.
* `first_name` - First-Name setting.
* `email_address` - Email-Address setting.
* `phone_number` - Phone-Number setting.
* `mobile_number` - Mobile-Number setting.
* `hidden` - Hidden setting.
* `domains` - Domains setting.
* `gui_global_menu_favorites` - Gui-Global-Menu-Favorites setting.
* `gui_vdom_menu_favorites` - Gui-Vdom-Menu-Favorites setting.
* `column` - Column setting.
* `status` - Status setting.
* `name` - Name setting.
* `layout_type` - Layout-Type setting.
* `permanent` - Permanent setting.
* `widget_table` - Widget-Table setting.
* `type` - Type setting.
* `admin_usergrp` - Admin-Usergrp setting.
* `password` - Password setting.
* `wildcard` - Wildcard setting.
* `accprofile_override` - Accprofile-Override setting.
* `fortiai` - Fortiai setting.
* `sshkey` - Sshkey setting.
* `passwd_set_time` - Passwd-Set-Time setting.
* `history_password_pos` - History-Password-Pos setting.
* `history_password0` - History-Password0 setting.
* `history_password1` - History-Password1 setting.
* `history_password2` - History-Password2 setting.
* `history_password3` - History-Password3 setting.
* `history_password4` - History-Password4 setting.
* `history_password5` - History-Password5 setting.
* `history_password6` - History-Password6 setting.
* `history_password7` - History-Password7 setting.
* `history_password8` - History-Password8 setting.
* `history_password9` - History-Password9 setting.
* `force_password_change` - Force-Password-Change setting.
* `feature_info_ver` - Feature-Info-Ver setting.
* `old_password` - Old-Password setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Admin can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_admin.labelname {mkey}
```
