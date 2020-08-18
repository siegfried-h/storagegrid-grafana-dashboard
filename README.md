# storagegrid-grafana-dashboard
This Repository contains a grafana dashboard in JSON format for Netapp StorageGrid 11.4 and later.

The dashboard uses the Prometheus data source and connects to the Prometheus service running on the Admin Node. For the dashboard to work, a fPVR needs to be created to open a firewall port on the Admin Node. Please contact your Netapp representative to open the fPVR request and receive the procedure to open the required port. Do not try to open the port on your own.

# Requirements:
Grafana 6.0.1
Prometheus 5.0.0
Port 9090 opened on Admin Node

# Installation instructions
In your Grafana instance, add a Prometheus data source and point it to the StorageGrid Admin Node. Make sure the required firewall port was opened by a Netapp representative. StorageGrid 11.4 does not support any authentication on Prometheus, so uncheck everything under "Auth" Section.
Once the Prometheus data source is created and working, import the JSON of the dashboard and select the just created data source.

# Links
This grafana dashboard is based on the following dashboard and was modified to make it work on StorageGrid version 11.4 and later:
https://grafana.com/grafana/dashboards/10440
