{
  "info": {
    "name": "AWS AppStream 2.0 API Start Fleet",
    "_postman_id": "5a6a1add-2bca-4b47-81c3-3fafa9746d79",
    "description": "Starts a fleet.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fleet",
      "item": [
        {
          "id": "8870574f-bfad-4968-a89f-581a8a0d4254",
          "name": "AssociateFleet",
          "request": {
            "url": "http://example.com/api/?Action=AssociateFleet?FleetName=FleetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associate a fleet to a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b807a081-a92c-48a5-b1cb-7388d9601470"
            }
          ]
        },
        {
          "id": "e61db589-1757-4288-bfba-da520b6688d8",
          "name": "CreateFleet",
          "request": {
            "url": "http://example.com/api/?Action=CreateFleet?ComputeCapacity=ComputeCapacity&Description=Description&DisconnectTimeoutInSeconds=DisconnectTimeoutInSeconds&DisplayName=DisplayName&ImageName=ImageName&InstanceType=InstanceType&MaxUserDurationInSeconds=MaxUserDurationInSeconds&Name=Name&VpcConfig=VpcConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d49488d-044f-4374-b0ea-b69b29338503"
            }
          ]
        },
        {
          "id": "56e3f17f-8698-4aed-83f6-31f0daf21bc2",
          "name": "CreateStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?Description=Description&DisplayName=DisplayName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44308a19-01e4-4c9a-8d74-0836a3994642"
            }
          ]
        },
        {
          "id": "5e30f6bf-d102-40bf-a787-16e6130f1291",
          "name": "DeleteFleet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFleet?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c841415-0250-40a3-b434-7226e2f74f5d"
            }
          ]
        },
        {
          "id": "c923cb64-9f88-47f0-8839-51b36ec9a151",
          "name": "DescribeFleets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFleets?Names=Names&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If fleet names are provided, this operation describes the specified fleets;\n            otherwise, all the fleets in the account are described."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5353264-e697-4990-abe1-712c48f17268"
            }
          ]
        },
        {
          "id": "4bae0ff8-c567-4b93-9601-cf1fc47886a7",
          "name": "DisassociateFleet",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateFleet?FleetName=FleetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a fleet from a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6883287c-9775-4228-b650-8930ec25bf1d"
            }
          ]
        },
        {
          "id": "740e9c08-f4bf-4751-b690-71a77facc373",
          "name": "ListAssociatedFleets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociatedFleets?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all fleets associated with the stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8be382dd-0159-4f28-a515-4e26d582bc5b"
            }
          ]
        },
        {
          "id": "55d94273-2475-4479-8f05-56ff5b4f4c04",
          "name": "StartFleet",
          "request": {
            "url": "http://example.com/api/?Action=StartFleet?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6158e0e-b101-43a4-8b50-8b9ae9cec078"
            }
          ]
        }
      ]
    },
    {
      "name": "URL",
      "item": [
        {
          "id": "1097cf73-f285-4dcd-aa21-337c3a09b546",
          "name": "CreateStreamingURL",
          "request": {
            "url": "http://example.com/api/?Action=CreateStreamingURL?ApplicationId=ApplicationId&FleetName=FleetName&SessionContext=SessionContext&StackName=StackName&UserId=UserId&Validity=Validity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a URL to start an AppStream 2."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10c35cd6-4354-4ee7-b2c4-47824bff0e31"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack",
      "item": [
        {
          "id": "57905e80-cb1c-43c0-9e25-a52d160accc9",
          "name": "DeleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c36ecd40-5d4b-4a6c-afb7-7f9b9fa26211"
            }
          ]
        },
        {
          "id": "9f05e56b-644f-44cf-b1a7-7060fac66bdb",
          "name": "ListAssociatedStacks",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociatedStacks?FleetName=FleetName&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all stacks to which the specified fleet is associated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca14d698-1998-4a24-b9e9-d39796520a37"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "2b4ac1e4-2801-409e-aac2-07b3458096df",
          "name": "DescribeImages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeImages?Names=Names",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8989e8d5-f5f5-468e-bad4-c126b52a725c"
            }
          ]
        }
      ]
    },
    {
      "name": "Sessions",
      "item": [
        {
          "id": "f371cac8-846e-4722-97c5-7ac207cb6b43",
          "name": "DescribeSessions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSessions?FleetName=FleetName&Limit=Limit&NextToken=NextToken&StackName=StackName&UserId=UserId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the streaming sessions for a stack and a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ae3a78b-dea3-41bb-8182-147c2c842f7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Stacks",
      "item": [
        {
          "id": "bbf42e67-4096-4fc3-8a66-87b4548532be",
          "name": "DescribeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?Names=Names&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If stack names are not provided, this operation describes the specified stacks;\n            otherwise, all stacks in the account are described."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9528d0d-b39a-41e7-baf9-ba73c2e7ed85"
            }
          ]
        }
      ]
    },
    {
      "name": "Session",
      "item": [
        {
          "id": "4d736b54-7e62-493b-8af5-0355ad82b4c9",
          "name": "ExpireSession",
          "request": {
            "url": "http://example.com/api/?Action=ExpireSession?SessionId=SessionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This operation immediately stops a streaming session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b846034d-d71a-4e11-827c-117c87427f0b"
            }
          ]
        }
      ]
    }
  ]
}