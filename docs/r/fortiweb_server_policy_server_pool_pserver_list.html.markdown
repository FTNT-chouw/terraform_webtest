---
subcategory: "FortiWEB Server Policy"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_server_policy_server_pool_pserver_list"
description: |-
  Configure FortiWEB server policy server pool pserver list configuration.
---

# fortiweb_server_policy_server_pool_pserver_list
Configure FortiWEB server policy server pool pserver list configuration.

## Example Usage
```hcl
resource "fortiweb_server_policy_server_pool_pserver_list" "test" {
	mkey = "test"
	sub_mkey = "1"
	status = "enable"
	server_type = "physical"
	ip = "1.1.1.1"
	port = 443
	conn_limit = 0
	proxy_protocol = "enable"
	proxy_protocol_version = "v1"
	http2 = "enable"
	ssl = "enable"
	client_certificate = "sign-p12"
	server_side_sni = "enable"
	server_certificate_verify = "enable"
	server_certificate_verify_policy = "test"
	server_certificate_verify_action = "alert_deny"
	use_ciphers_group = "disable"
	tls_v10 = "disable"
	tls_v11 = "disable"
	tls_v12 = "enable"
	tls_v13 = "enable"
	ssl_cipher = "medium"
	rfc7919_comply = "disable"
	recover = 123
	warm_up = 1234
	warm_rate = 10
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The ID of the server policy server pool pserver list entry.
* `id` - Id setting.
* `server_type` - Server-Type setting.
* `ip` - Ip setting.
* `domain` - Domain setting.
* `adfs_username` - Adfs-Username setting.
* `adfs_password` - Adfs-Password setting.
* `sdn_addr_type` - Sdn-Addr-Type setting.
* `sdn` - Sdn setting.
* `filter` - Filter setting.
* `port` - Port setting.
* `weight` - Weight setting.
* `status` - Status setting.
* `server_id` - Server-Id setting.
* `backup_server` - Backup-Server setting.
* `proxy_protocol` - Proxy-Protocol setting.
* `proxy_protocol_version` - Proxy-Protocol-Version setting.
* `ssl` - Ssl setting.
* `implicit_ssl` - Implicit Ssl setting.
* `ssl_quiet_shutdown` - Ssl-Quiet-Shutdown setting.
* `ssl_session_timeout` - Ssl-Session-Timeout setting.
* `server_side_sni` - Server-Side-Sni setting.
* `multi_certificate` - Multi-Certificate setting.
* `certificate` - Certificate setting.
* `certificate_group` - Certificate-Group setting.
* `certificate_type` - Certificate-Type setting.
* `lets_certificate` - Lets-Certificate setting.
* `intermediate_certificate_group` - Intermediate-Certificate-Group setting.
* `certificate_verify` - Certificate-Verify setting.
* `client_certificate_proxy` - Client-Certificate-Proxy setting.
* `client_certificate_proxy_sign_ca` - Client-Certificate-Proxy-Sign-Ca setting.
* `client_certificate` - Client-Certificate setting.
* `server_certificate_verify` - Server-Certificate-Verify setting.
* `server_certificate_verify_policy` - Server-Certificate-Verify-Policy setting.
* `server_certificate_verify_action` - Server-Certificate-Verify-Action setting.
* `session_ticket_reuse` - Session-Ticket-Reuse setting.
* `session_id_reuse` - Session-Id-Reuse setting.
* `sni` - Sni setting.
* `sni_certificate` - Sni-Certificate setting.
* `sni_strict` - Sni-Strict setting.
* `urlcert` - Urlcert setting.
* `urlcert_group` - Urlcert-Group setting.
* `urlcert_hlen` - Urlcert-Hlen setting.
* `use_ciphers_group` - Use-Ciphers-Group setting.
* `ssl_ciphers_group` - Ssl-Ciphers-Group setting.
* `tls_v10` - Tls-V10 setting.
* `tls_v11` - Tls-V11 setting.
* `tls_v12` - Tls-V12 setting.
* `tls_v13` - Tls-V13 setting.
* `ssl_noreg` - Ssl-Noreg setting.
* `ssl_cipher` - Ssl-Cipher setting.
* `ssl_custom_cipher` - Ssl-Custom-Cipher setting.
* `tls13_custom_cipher` - Tls13-Custom-Cipher setting.
* `rfc7919_comply` - Rfc7919-Comply setting.
* `supported_groups` - Supported-Groups setting.
* `tls_pqc_support` - Tls-Pqc-Support setting.
* `tls_pqc_groups` - Tls-Pqc-Groups setting.
* `hsts_header` - Hsts-Header setting.
* `hsts_max_age` - Hsts-Max-Age setting.
* `hsts_include_subdomains` - Hsts-Include-Subdomains setting.
* `hsts_preload` - Hsts-Preload setting.
* `hpkp_header` - Hpkp-Header setting.
* `client_certificate_forwarding` - Client-Certificate-Forwarding setting.
* `client_certificate_forwarding_sub_header` - Client-Certificate-Forwarding-Sub-Header setting.
* `client_certificate_forwarding_cert_header` - Client-Certificate-Forwarding-Cert-Header setting.
* `health_check_inherit` - Health-Check-Inherit setting.
* `health` - Health setting.
* `conn_limit` - Conn-Limit setting.
* `recover` - Recover setting.
* `warm_up` - Warm-Up setting.
* `warm_rate` - Warm-Rate setting.
* `http2` - Http2 setting.
* `http2_window_size` - Http2-Window-Size setting.
* `hlck_domain` - Hlck-Domain setting.
* `http_https_adaptive` - Http-Https-Adaptive setting.
* `http_port` - Http-Port setting.
* `https_port` - Https-Port setting.
* `enforce_trust_establishment` - Enforce-Trust-Establishment setting.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Server Policy Server Pool Pserver List can be imported using any of these accepted formats:
```
$ terraform import fortiweb_server_policy_server_pool_pserver_list.labelname {mkey}
```
