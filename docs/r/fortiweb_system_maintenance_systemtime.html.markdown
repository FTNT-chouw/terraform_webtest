---
subcategory: "FortiWEB System"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_system_maintenance_systemtime"
description: |-
  Configure FortiWEB system maintenance systemtime configuration.
---

# fortiweb_system_maintenance_systemtime
Configure FortiWEB system maintenance systemtime configuration.

## Example Usage
```hcl
resource "fortiweb_system_maintenance_systemtime" "test" {
	daylightsaving = 0
	timezone = 3
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the system ha entry.
* `mode` - Mode setting.
* `group_id` - Group-Id setting.
* `group_name` - Group-Name setting.
* `priority` - Priority setting.
* `override` - Override setting.
* `network_type` - Network-Type setting.
* `tunnel_local` - Tunnel-Local setting.
* `tunnel_peer` - Tunnel-Peer setting.
* `hbdev` - Hbdev setting.
* `hbdev_backup` - Hbdev-Backup setting.
* `boot_time` - Boot-Time setting.
* `hb_interval` - Hb-Interval setting.
* `hb_lost_threshold` - Hb-Lost-Threshold setting.
* `arps` - Arps setting.
* `arp_interval` - Arp-Interval setting.
* `monitor` - Monitor setting.
* `key` - Key setting.
* `lacp_ha_slave` - Lacp-Ha-Slave setting.
* `ha_mgmt_status` - Ha-Mgmt-Status setting.
* `ha_mgmt_interface` - Ha-Mgmt-Interface setting.
* `session_pickup` - Session-Pickup setting.
* `session_sync_dev` - Session-Sync-Dev setting.
* `session_sync_broadcast` - Session-Sync-Broadcast setting.
* `session_warm_up` - Session-Warm-Up setting.
* `schedule` - Schedule setting.
* `weight_1` - Weight-1 setting.
* `weight_2` - Weight-2 setting.
* `weight_3` - Weight-3 setting.
* `weight_4` - Weight-4 setting.
* `weight_5` - Weight-5 setting.
* `weight_6` - Weight-6 setting.
* `weight_7` - Weight-7 setting.
* `weight_8` - Weight-8 setting.
* `link_failed_signal` - Link-Failed-Signal setting.
* `l7_persistence_sync` - L7-Persistence-Sync setting.
* `eip_addr` - Eip-Addr setting.
* `eip_aid` - Eip-Aid setting.
* `ha_eth_type` - Ha-Eth-Type setting.
* `hc_eth_type` - Hc-Eth-Type setting.
* `l2ep_eth_type` - L2Ep-Eth-Type setting.
* `server_policy_hlck` - Server-Policy-Hlck setting.
* `multi_cluster` - Multi-Cluster setting.
* `multi_cluster_group` - Multi-Cluster-Group setting.
* `multi_cluster_switch_by` - Multi-Cluster-Switch-By setting.
* `multi_cluster_move_primary_cluster` - Multi-Cluster-Move-Primary-Cluster setting.
* `encryption` - Encryption setting.
* `cluster_arp` - Cluster-Arp setting.
* `sdn_connector` - Sdn-Connector setting.
* `lb_name` - Lb-Name setting.
* `lb_ocid` - Lb-Ocid setting.
* `lb_gcp` - Lb-Gcp setting.
* `hlck_sync` - Hlck-Sync setting.
* `hlck_period_sync` - Hlck-Period-Sync setting.
* `hlck_period_timeout` - Hlck-Period-Timeout setting.
* `distribution` - Distribution setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

System Maintenance Systemtime can be imported using any of these accepted formats:
```
$ terraform import fortiweb_system_maintenance_systemtime.labelname {mkey}
```
