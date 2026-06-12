1. Use the idrac get_error_and_event_registry tool to get details about the alerts.
2. Get the top 10 lifecycle logs of severity Critical.
3. Discover the related metrics using the prometheus discover_metrics tool, then query them using the get_metric_analysis tool setting window hours to 24.
4. In the case of a potential system crash, use the idrac export_server_screen_shot tool to provide a summary of the ServerScreenShot image <|image|>