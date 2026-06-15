---
name: telemetry-metric-browser
description: Browse MetricReportDefinitions and fetch selected report details.
version: 1.0.0
---

1. Start at /redfish/v1/TelemetryService/MetricReportDefinitions on {host}.
2. Use idrac get_redfish_uri to list metric report definition links.
3. Present the user a prompt to select which metric report definitions to retrieve.
4. Retrieve details for the selected definitions in parallel using idrac get_redfish_uri and return aggregated results.
