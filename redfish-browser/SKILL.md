---
name: redfish-browser
description: Walk Redfish API directories and fetch linked resources in parallel.
version: 1.0.0
---

1. Start a Redfish API directory walk at /redfish/v1/Chassis/System.Embedded.1 on {host}.
2. Use the idrac get_redfish_uri tool to request the resource and parse JSON for linkable members.
3. Return a grouped list of links to follow next and prompt the user to select which groups or links to explore.
4. For the selected links, make requests in parallel (batching if necessary) and collect the responses into a single aggregated result. Use idrac get_redfish_uri on each link.
