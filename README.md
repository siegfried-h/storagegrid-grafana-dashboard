# storagegrid-grafana-dashboard
This Repository includes a grafana dashboard for Netapp StorageGrid 11.4 and later

The dashboard connects to the Prometheus service running on the Admin node. For the dashboard to work, a fPVR needs to be created to open a firewall port on the admin node. Please contact your Netapp representative to open the fPVR and receive the procedure to open the port.

# Requirements:
Grafana 6.0.1
Prometheus 5.0.0
Port 9090 opened on Admin Node

# Installation instructions
In your Grafana instance, add a Prometheus data source and point it to the StorageGrid Admin Node. Make sure the required firewall port was opened by a Netapp representative. StorageGrid 11.4 does not support any authentification on Prometheus and uses http to port 9090, so uncheck everything under "Auth" Section.
Once the Prometheus Datasource is created and working, import the JSON of the dashboard and select the just created Datasource.

# Links
This grafana dashboard is based on the following dashboard that was modified to make it work on StorageGrid 11.4:
https://grafana.com/grafana/dashboards/10440
