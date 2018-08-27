swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/proxy/anomalies/report:
    get:
      summary: Anomalies Report
      description: Retrieves Anomalies Report
      operationId: retrieveReportUsingGET
      x-api-path-slug: v1proxyanomaliesreport-get
      parameters:
      - in: query
        name: analysisId
        description: Analysis Id
      - in: query
        name: dataSourceName
        description: Data Source name
      - in: query
        name: fromAnomaly
        description: Fetch from Anomaly in Analysis
      - in: query
        name: numOfTopFeatures
        description: Number of top features to fetch
      - in: query
        name: toAnomaly
        description: Fetch up to Anomaly in Analysis
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Anomalies
      - Report