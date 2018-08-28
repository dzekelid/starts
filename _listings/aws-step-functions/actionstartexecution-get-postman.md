{
  "info": {
    "name": "AWS Step Functions API Start Execution",
    "_postman_id": "d86ae756-19e1-4658-95c3-8e9cebac58a3",
    "description": "Starts a state machine execution.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "State Machine",
      "item": [
        {
          "id": "95900786-e5ac-42ad-adb5-1c00705e1d68",
          "name": "createStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=CreateStateMachine?definition=definition&name=name&roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f42cbf7e-664c-43a8-857a-6fdf70946e68"
            }
          ]
        },
        {
          "id": "9e60a59c-0a2e-42f2-9f9d-b668d7fb847f",
          "name": "deleteStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStateMachine?stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ced81efd-510d-43b5-9c03-821a9332aeb0"
            }
          ]
        },
        {
          "id": "de8914b7-dd47-43d1-bda8-d62d2dfb074e",
          "name": "describeStateMachine",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStateMachine?stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a state machine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93533dba-e592-4010-a23c-006760af1215"
            }
          ]
        },
        {
          "id": "ca3b34ff-9de0-49f2-86c4-e4c3c6d68317",
          "name": "listExecutions",
          "request": {
            "url": "http://example.com/api/?Action=ListExecutions?maxResults=maxResults&nextToken=nextToken&stateMachineArn=stateMachineArn&statusFilter=statusFilter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a state machine that meet the filtering criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d44d6ab4-9a47-419a-8e1a-626d503bb100"
            }
          ]
        },
        {
          "id": "547d8736-4f0a-4e12-aa28-e1d0984855df",
          "name": "listStateMachines",
          "request": {
            "url": "http://example.com/api/?Action=ListStateMachines?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the existing state machines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c1b373-d0e4-41db-8a5e-cc4edda5ab1c"
            }
          ]
        },
        {
          "id": "6b77f28f-e6cd-4bd6-907c-47f0b92668b9",
          "name": "startExecution",
          "request": {
            "url": "http://example.com/api/?Action=StartExecution?input=input&name=name&stateMachineArn=stateMachineArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a state machine execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "476affe7-7e07-4d59-9342-8209015976a7"
            }
          ]
        }
      ]
    }
  ]
}