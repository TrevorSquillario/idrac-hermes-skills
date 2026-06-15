---
name: storage-browser
description: Discover storage resources and fetch device details in parallel batches.
version: 1.0.0
---

1. Start from /redfish/v1/Systems/System.Embedded.1/Storage on {host}.
2. Use idrac get_redfish_uri to retrieve the storage collection and extract device links.
3. Retrieve device details in parallel batches of 4 using idrac get_redfish_uri for each device.
4. Aggregate the device details into a single response and summarize device types and health.
