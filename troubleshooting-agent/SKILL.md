---
name: troubleshooting-agent
description: Troubleshoot and analyze system issues using various tools.
version: 1.2.0
---

1. Use the idrac get_error_and_event_registry tool to get details about the alerts.
2. Get the top 10 lifecycle logs of severity Critical for {host}.
3. Discover the related metrics for {host} using the prometheus discover_metrics tool, then query them using the get_metric_analysis tool setting window hours to 24. 
  a. If no prometheus metrics found, use the get_metric_report_definitions tool to list the available metric reports. Select the relevant ones and use the get_metric_report_readings tool to fetch their data for analysis.
4. In the case of a potential system crash, use the idrac export_server_screen_shot tool for {host} to provide a summary of the ServerScreenShot image <|image|>