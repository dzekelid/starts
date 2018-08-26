{
  "info": {
    "name": "AWS Server Migration Service API Start On Demand Replication Run",
    "_postman_id": "faca622b-fc7c-4fe7-8e29-4a11d9d71181",
    "description": "The start-on-demand-replication-run API is used to start a ReplicationRun on demand (in addition to those that are scheduled based on your frequency).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Replication Jobs",
      "item": [
        {
          "id": "7bbca544-199e-4f52-b071-0a8af01378f4",
          "name": "createReplicationJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationJob?description=description&frequency=frequency&licenseType=licenseType&roleName=roleName&seedReplicationTime=seedReplicationTime&serverId=serverId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The create-replication-job API is used to create a ReplicationJob to replicate a server on AWS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aefc9411-1889-4516-9c4d-2c409015d85d"
            }
          ]
        },
        {
          "id": "b726fb5e-8f57-4a73-885b-c7ef4d98c3d3",
          "name": "deleteReplicationJob",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationJob?replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The delete-replication-job API is used to delete a ReplicationJob, resulting in no further ReplicationRuns."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63a289b5-f84b-482a-a319-7f33450e669c"
            }
          ]
        },
        {
          "id": "82f3f65a-f5de-46ca-8151-417608f5ff3c",
          "name": "getReplicationJobs",
          "request": {
            "url": "http://example.com/api/?Action=GetReplicationJobs?maxResults=maxResults&nextToken=nextToken&replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-replication-jobs API will return all of your ReplicationJobs and their details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "529c9cda-d398-477a-b297-c0b71f87e396"
            }
          ]
        }
      ]
    },
    {
      "name": "Server Catalog",
      "item": [
        {
          "id": "9fa932d4-d6db-4667-ac9b-196e0c479442",
          "name": "deleteServerCatalog",
          "request": {
            "url": "http://example.com/api/?Action=DeleteServerCatalog",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The delete-server-catalog API clears all servers from your server catalog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5f6bff5-88da-4121-9e4f-5dbfe0727d89"
            }
          ]
        },
        {
          "id": "5952f7bd-9873-4b5d-a033-65fe130e9808",
          "name": "importServerCatalog",
          "request": {
            "url": "http://example.com/api/?Action=ImportServerCatalog",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The import-server-catalog API is used to gather the complete list of on-premises servers on your premises."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee6e21c9-140f-456b-9152-e05d9b946aad"
            }
          ]
        }
      ]
    },
    {
      "name": "Connectors",
      "item": [
        {
          "id": "9b3a5219-92e3-4a97-b0a2-f8ed4d78365b",
          "name": "disassociateConnector",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateConnector?connectorId=connectorId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The disassociate-connector API will disassociate a connector from the Server Migration Service, rendering it unavailable to support replication jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3faba05b-22c0-48ad-bc0c-36960bf26257"
            }
          ]
        },
        {
          "id": "4bdcf1ba-faf3-47fc-bef1-24a569da0158",
          "name": "getConnectors",
          "request": {
            "url": "http://example.com/api/?Action=GetConnectors?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-connectors API returns a list of connectors that are registered with the Server Migration Service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe8711d3-3f3f-4ada-8c92-41f22e5f41fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Runs",
      "item": [
        {
          "id": "fce9a7ef-e6b5-4122-8adb-33c13e269477",
          "name": "getReplicationRuns",
          "request": {
            "url": "http://example.com/api/?Action=GetReplicationRuns?maxResults=maxResults&nextToken=nextToken&replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-replication-runs API will return all ReplicationRuns for a given ReplicationJob."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20908bf9-925c-47f1-a856-2aab3311b6bc"
            }
          ]
        },
        {
          "id": "02022c55-5e86-4c3c-94e4-9f4287fdd606",
          "name": "startOnDemandReplicationRun",
          "request": {
            "url": "http://example.com/api/?Action=StartOnDemandReplicationRun?description=description&replicationJobId=replicationJobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The start-on-demand-replication-run API is used to start a ReplicationRun on demand (in addition to those that are scheduled based on your frequency)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00fd89bf-2762-4be8-bdc5-ba74951806fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Servers",
      "item": [
        {
          "id": "2b6992ad-20d3-486a-aea5-01fab361bac6",
          "name": "getServers",
          "request": {
            "url": "http://example.com/api/?Action=GetServers?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The get-servers API returns a list of all servers in your server catalog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1164bdd3-8a7e-4d00-84c7-3701488d2017"
            }
          ]
        }
      ]
    }
  ]
}