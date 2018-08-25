{
  "info": {
    "name": "Predix ThetaRay Predix Service Anomalies Report",
    "_postman_id": "f83558ca-089f-47ba-a53a-5c9e643c0610",
    "description": "Retrieves Anomalies Report",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Proxy",
      "item": [
        {
          "id": "bebe0e90-b1ac-4e70-be44-36b61c89af9d",
          "name": "retrieveNewUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/analyses",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get list of Analyses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b658ec8-2fc9-468e-9a5a-0471877a2b81"
            }
          ]
        },
        {
          "id": "da6781e4-3bce-4f81-8368-b8d2490f72d1",
          "name": "retrieveReportUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/anomalies/report?analysisId=%7B%7D&dataSourceName=%7B%7D&fromAnomaly=%7B%7D&numOfTopFeatures=%7B%7D&toAnomaly=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves Anomalies Report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a500b3c8-4403-4c99-8960-beff4c9911ef"
            }
          ]
        }
      ]
    }
  ]
}