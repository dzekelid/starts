{
  "info": {
    "name": "import.io Post Extractor Extractorid Start",
    "_postman_id": "ca03bd80-001f-4c62-ab10-7c56755abff7",
    "description": "Launch a crawl from an extractor that a user owns..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Extractor",
      "item": [
        {
          "id": "c5ca061e-8727-49d2-baf4-5f87b34595a9",
          "name": "getExtractorExtractorCsvLatest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/csv/latest"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the latest crawl run results as a csv."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40c0633a-769c-4b86-81be-b6aab382459b"
            }
          ]
        },
        {
          "id": "2198f8b9-7a91-49ed-8608-fd69896eda26",
          "name": "getExtractorExtractorJsonLatest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/json/latest"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the latest crawl run results as json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9615da6-f86e-4a3a-8ab6-a4190ed4f5f0"
            }
          ]
        },
        {
          "id": "5007bbd9-c97c-4714-a594-88bac96f01f5",
          "name": "getExtractorExtractor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId"
              ],
              "query": [
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query by extractor endpoint, adhoc runs only.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53b98daa-594a-4311-81ec-d0a5477cd6fb"
            }
          ]
        },
        {
          "id": "9544ce11-6c8d-4cef-bcfe-23bd77a678f7",
          "name": "getExtractorExtractorRuns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/runs"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a feed of the runs performed on an extractor."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f58511e3-aa19-4ef8-8f5e-fd162e4fd63c"
            }
          ]
        },
        {
          "id": "12325e4d-c84c-452f-ad5a-5d20e62347c1",
          "name": "postExtractorExtractorCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/cancel"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Cancel an existing crawl.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "237e953d-74e9-4796-8594-189a46312d54"
            }
          ]
        },
        {
          "id": "eba8bf8c-416c-4977-a3be-e80f12ac0460",
          "name": "postExtractorExtractorStart",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/start"
              ],
              "query": [
                {
                  "key": "loginSessionId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Launch a crawl from an extractor that a user owns.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4685f4f-23b1-47ce-a187-cbcbbcbd3e79"
            }
          ]
        }
      ]
    }
  ]
}