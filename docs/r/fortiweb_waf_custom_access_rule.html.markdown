---
subcategory: "FortiWEB WAF"
layout: "fortiweb"
page_title: "FortiWEB: fortiweb_waf_custom_access_rule"
description: |-
  Configure FortiWEB waf custom access rule configuration.
---

# fortiweb_waf_custom_access_rule
Configure FortiWEB waf custom access rule configuration.

## Example Usage
```hcl
resource "fortiweb_waf_custom_access_rule" "test" {
	mkey = "test"
	action = "alert"
	block_period = 600
	severity = "Medium"
	trigger = "test"
	bot_confirmation = "enable"
	bot_recognition = "captcha-puzzle-enforcement"
	max_attempt_times = 3
	validation_timeout = 20
}

```

## Argument Reference

The following arguments are supported:

* `vdom` - Specifies the vdom to which the data source will be applied when the FortiWEB unit is running in VDOM mode. Only one vdom can be specified. If you want to inherit the vdom configuration of the provider, please do not set this parameter.
* `mkey` - The name of the waf custom access rule entry.
* `action` - Select which action the FortiWeb appliance will take when it detects a violation of the rule.
* `block_period` - Type the number of seconds that you want to block subsequent requests from the client.
* `severity` - Select which severity level the FortiWeb appliance will use when it logs a violation of the rule. Valid values: Informative, Low, Medium, High.
* `trigger` - Select which trigger.
* `bot_confirmation` - Enable to confirm if the client is indeed a bot.
* `bot_recognition` - Real Browser Enforcement, CAPTCHA Enforcement, Puzzle CAPTCHA Enforcement, reCAPTCHA Enforcement, reCAPTCHA v3 Enforcement.
* `max_attempt_times` - Enter the maximum number of attempts that a client may attempt to fulfill a CAPTCHA/Puzzle CAPTCHA Enforcement request.
* `validation_timeout` - Enter the maximum amount of time (in seconds) that FortiWeb waits for results from the client.

## Attribute Reference

In addition to all the above arguments, the following attributes are exported:
* `id` - an identifier for the resource with format {{mkey}}.

## Import

Waf Custom Access Rule can be imported using any of these accepted formats:
```
$ terraform import fortiweb_waf_custom_access_rule.labelname {mkey}
```
