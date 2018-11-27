# Kibana dashboard
Contains all the Kibana dashboards files. Each dasboard information is exported with information related with the indexes used in the visualization and the visualization itselft.  

### Export kibana dashboards
Once a visualization is created it is possible to exported using the below curl command.
```
curl "http://kibana:5601/api/kibana/dashboards/export?dashboard=<dashboard-id>" > <dashobard_name>.json
```

## Import Kibana dashboard
In order to import a dashboard configuration the below script can be used.
```
curl -X POST -H "Content-Type: application/json" -H "kbn-xsrf: true" http://kibana:5601/api/kibana/dashboards/import -d @<dashboard_name>.json
```

## Cartridge adop-cartridge-elk
See more details in the project: [adop-cartridge-elk](https://github.com/RobeDevOps/adop-cartridge-elk)
