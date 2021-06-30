# storagegrid-grafana-dashboard
This Repository contains a grafana dashboard in JSON format for Netapp StorageGrid 11.4 and later.

The dashboard uses the Prometheus data source and connects to the Prometheus service running on the Admin Node. The performance data stays on the Admin node and will not be imported in your grafana server.

# Requirements:
StorageGrid 11.5 and later
Grafana 6.0.1 or later
Prometheus 5.0.0 or later
Port 9091 opened between Grafana Server and Admin Node

# Installation instructions
In your Grafana instance, add a Prometheus data source and point it to the StorageGrid Admin Node. Configure the datasource like described here:
https://docs.netapp.com/sgws-115/topic/com.netapp.doc.sg-admin/GUID-3F909B3F-D1E3-41E0-8886-6F62CE38750B.html
Once the Prometheus data source is created and working, import the JSON of the dashboard and select the just created data source.
