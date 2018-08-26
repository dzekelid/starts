{
  "info": {
    "name": "AWS Inspector API Start Assessment Run",
    "_postman_id": "f92e6f88-352f-45f5-89bb-a29a6a691e50",
    "description": "Starts the assessment run specified by the ARN of the assessment template.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "139c95dd-80e0-4220-8d3f-1f42c04111f5",
          "name": "addAttributesToFindings",
          "request": {
            "url": "http://example.com/api/?Action=AddAttributesToFindings?attributes=attributes&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns attributes (key and value pairs) to the findings that are specified by the\n         ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4de6078a-9000-4e45-9c76-5dc0fc0837f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Targets",
      "item": [
        {
          "id": "8139cf63-6c30-48b0-9b8d-70dcb22610c6",
          "name": "createAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTarget?assessmentTargetName=assessmentTargetName&resourceGroupArn=resourceGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new assessment target using the ARN of the resource group that is generated\n         by."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9152bab-d958-40d7-b3bc-510b7c5777e3"
            }
          ]
        },
        {
          "id": "c9ba7178-4fd4-4ff3-958e-2723b5c0511f",
          "name": "deleteAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTarget?assessmentTargetArn=assessmentTargetArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment target that is specified by the ARN of the assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "205599b4-06b6-4706-9ce5-a3d2965d0188"
            }
          ]
        },
        {
          "id": "8fc8e6f1-512f-44d8-ad0c-29d97121010c",
          "name": "describeAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTargets?assessmentTargetArns=assessmentTargetArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment targets that are specified by the ARNs of the assessment\n         targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67add558-7ea7-4567-ac52-412191573f63"
            }
          ]
        },
        {
          "id": "d2a8e1dc-f710-4018-adb5-c8a4d170f8dc",
          "name": "listAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTargets?filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the ARNs of the assessment targets within this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28452b66-0254-4fab-9ca3-dce98928c04a"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Templates",
      "item": [
        {
          "id": "f846e6aa-629e-403a-9fbb-4acee07d2337",
          "name": "createAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTemplate?assessmentTargetArn=assessmentTargetArn&assessmentTemplateName=assessmentTemplateName&durationInSeconds=durationInSeconds&rulesPackageArns=rulesPackageArns&userAttributesForFindings=userAttributesForFindings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an assessment template for the assessment target that is specified by the ARN\n         of the assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "257dbd18-2574-4ff7-ad12-678d1454cc1e"
            }
          ]
        },
        {
          "id": "016743da-d777-4532-aaba-db00321bccae",
          "name": "deleteAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTemplate?assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment template that is specified by the ARN of the assessment\n         template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f13c0558-0f53-4a71-82a9-e69f4133086e"
            }
          ]
        },
        {
          "id": "c4d6a8e4-d6f4-4516-b4f0-e1d24b9d282e",
          "name": "describeAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTemplates?assessmentTemplateArns=assessmentTemplateArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment templates that are specified by the ARNs of the assessment\n         templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c2006b5-84b6-452e-a214-fd9fc6460d6c"
            }
          ]
        },
        {
          "id": "5a3346ff-d2f2-458b-a5fa-b8a692828c2a",
          "name": "listAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTemplates?assessmentTargetArns=assessmentTargetArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment templates that correspond to the assessment targets that are\n         specified by the ARNs of the assessment targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67e99130-0fea-4512-953a-100e2c84edf4"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Groups",
      "item": [
        {
          "id": "4c0d7492-38a4-4975-877f-017f06343996",
          "name": "createResourceGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateResourceGroup?resourceGroupTags=resourceGroupTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a resource group using the specified set of tags (key and value pairs) that\n         are used to select the EC2 instances to be included in an Amazon Inspector assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7aaf20b-7cd4-499d-a9f6-a5e88251b506"
            }
          ]
        },
        {
          "id": "49af36aa-1764-48ce-acb0-966d34e7c26a",
          "name": "describeResourceGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeResourceGroups?resourceGroupArns=resourceGroupArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the resource groups that are specified by the ARNs of the resource\n         groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2796bc8-f1ca-4800-8e77-13e04cbbc462"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Runs",
      "item": [
        {
          "id": "103f3216-ff98-4d9e-9848-88e9a88a9109",
          "name": "deleteAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3d98069-400c-496e-b728-49e20188d60f"
            }
          ]
        },
        {
          "id": "ebcb8a80-5da6-4fd3-9fd5-c2714cbefd23",
          "name": "describeAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentRuns?assessmentRunArns=assessmentRunArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment runs that are specified by the ARNs of the assessment\n         runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd068342-5956-4ad3-82f5-bca1b1acf830"
            }
          ]
        },
        {
          "id": "bc876563-26df-420f-86da-b5baaf5211bb",
          "name": "listAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRuns?assessmentTemplateArns=assessmentTemplateArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment runs that correspond to the assessment templates that are\n         specified by the ARNs of the assessment templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "892db82c-2c1d-417c-9d77-b2ee054860ed"
            }
          ]
        },
        {
          "id": "b8ae3ae7-04cd-4fa7-a949-106f5d08170f",
          "name": "startAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StartAssessmentRun?assessmentRunName=assessmentRunName&assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the assessment run specified by the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "024dc84f-34de-4c64-acb2-e431356328a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Cross Account Access Roles",
      "item": [
        {
          "id": "1f446dc9-497e-4232-8a5b-13bb33516105",
          "name": "describeCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCrossAccountAccessRole?registeredAt=registeredAt&roleArn=roleArn&valid=valid",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the IAM role that enables Amazon Inspector to access your AWS\n         account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1af06665-94d3-49e2-92fc-f555a0d816ae"
            }
          ]
        },
        {
          "id": "643c6d97-01af-41af-add9-ecd62b0d0db6",
          "name": "registerCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=RegisterCrossAccountAccessRole?roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers the IAM role that Amazon Inspector uses to list your EC2 instances at the\n         start of the assessment run or when you call the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e2752ad-4194-4c1b-9a33-4f6b54a960e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "1b0404e6-4872-4aaf-b9de-c89355503a16",
          "name": "describeFindings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFindings?findingArns=findingArns&locale=locale",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the findings that are specified by the ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca085535-e9d5-4e19-905c-1dd3d8ba3639"
            }
          ]
        },
        {
          "id": "f99a24cb-3ad1-4828-a469-354d1efa8fec",
          "name": "listFindings",
          "request": {
            "url": "http://example.com/api/?Action=ListFindings?assessmentRunArns=assessmentRunArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists findings that are generated by the assessment runs that are specified by the\n         ARNs of the assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "699026db-51e5-4bcd-aa89-8e6f77fcbda8"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules Packages",
      "item": [
        {
          "id": "632aa9d5-1d7f-40a9-b214-4101df8c8a3d",
          "name": "describeRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRulesPackages?locale=locale&rulesPackageArns=rulesPackageArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the rules packages that are specified by the ARNs of the rules\n         packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ada8dfc2-c7a4-487e-a3c1-f9283b6e52a8"
            }
          ]
        },
        {
          "id": "b3c3fb81-d668-4e43-8378-93e02ca5c02c",
          "name": "listRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=ListRulesPackages?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all available Amazon Inspector rules packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdd42c47-4ea9-4d54-9697-7842d0712c6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Telemetry Metadata",
      "item": [
        {
          "id": "f1bf775c-15eb-4f2f-a3df-39a878bb04e1",
          "name": "getTelemetryMetadata",
          "request": {
            "url": "http://example.com/api/?Action=GetTelemetryMetadata?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the data that is collected for the specified assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15ae0b8d-61bb-47d2-902d-59d037e4814b"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Run Agents",
      "item": [
        {
          "id": "3dd26a30-9e59-41ff-91c0-2ba316adf58e",
          "name": "listAssessmentRunAgents",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRunAgents?assessmentRunArn=assessmentRunArn&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the agents of the assessment runs that are specified by the ARNs of the\n         assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7baf0fec-6431-4608-938d-4cac0e6312db"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "bcc640ad-12f6-4d9f-acaa-8173f893dab1",
          "name": "listEventSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListEventSubscriptions?maxResults=maxResults&nextToken=nextToken&resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the event subscriptions for the assessment template that is specified by\n         the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "164529c3-56ea-4e16-a815-351c7007ace9"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags For Resources",
      "item": [
        {
          "id": "758bf82c-0a49-4c74-bbe6-b99cf19bbac0",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags associated with an assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e196f8a6-b660-49df-a414-f81ce050cecb"
            }
          ]
        },
        {
          "id": "176155dc-cc9e-46ed-a255-f107f40921b1",
          "name": "setTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=SetTagsForResource?resourceArn=resourceArn&tags=tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets tags (key and value pairs) to the assessment template that is specified by the\n         ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c000592c-dd87-4f40-8802-f0ab62640259"
            }
          ]
        }
      ]
    },
    {
      "name": "Agents",
      "item": [
        {
          "id": "22e73a16-b509-4491-8040-6c310d0c16e9",
          "name": "previewAgents",
          "request": {
            "url": "http://example.com/api/?Action=PreviewAgents?maxResults=maxResults&nextToken=nextToken&previewAgentsArn=previewAgentsArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Previews the agents installed on the EC2 instances that are part of the specified\n         assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e1a3fcf-3b40-4dd4-b8d9-0c00d83f9039"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes From Findings",
      "item": [
        {
          "id": "ffe5bbe2-08ad-4807-a179-5b9d5af68a8e",
          "name": "removeAttributesFromFindings",
          "request": {
            "url": "http://example.com/api/?Action=RemoveAttributesFromFindings?attributeKeys=attributeKeys&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes entire attributes (key and value pairs) from the findings that are specified\n         by the ARNs of the findings where an attribute with the specified key exists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce3ecaad-e80e-4117-8c7c-34a693a272a5"
            }
          ]
        }
      ]
    }
  ]
}