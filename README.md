# Export Kibana dashboard

curl "kibana:5601/api/kibana/dashboards/export?dashboard=<dashboard-id>" > export.json

# Import Kibana dashboard
curl -X POST -H "Content-Type: application/json" -H "kbn-xsrf: true" http://kibana:5601/api/kibana/dashboards/import -d @export.json