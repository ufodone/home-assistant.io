---
title: Tailscale
description: Instructions on how to integrate Tailscale within Home Assistant.
ha_category:
  - Binary Sensor
  - Sensor
  - Network
ha_release: 2021.12
ha_iot_class: Cloud Polling
ha_config_flow: true
ha_codeowners:
  - '@frenck'
ha_domain: tailscale
ha_platforms:
  - binary_sensor
  - diagnostics
  - sensor
ha_quality_scale: platinum
---

The Tailscale integration integrates the [Tailscale](https://www.tailscale.com) API
with Home Assistant; giving you the possibility to monitor and automate on
the state of the devices in your Tailscale VPN network (Tailnet).

Please, note that this integration integrates with data from the Tailscale API,
it is not a Tailscale client itself, and thus add Home Assistant to your
Tailscale VPN network.

## Prerequisites

To use the Tailscale integration, you will need to obtain an API key,
you can create one in the [Tailscale Admin Panel](https://login.tailscale.com/admin/settings/authkeys).

Additionally, you will need to know the Tailnet name of your Tailscale network.
You can find it in the top left corner in the [Tailscale Admin Panel](https://login.tailscale.com/admin/settings/authkeys)
(beside the Tailscale logo).

{% include integrations/config_flow.md %}
