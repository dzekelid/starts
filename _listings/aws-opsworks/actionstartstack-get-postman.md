{
  "info": {
    "name": "AWS OpsWorks API Start Stack",
    "_postman_id": "af998da8-9ea5-4f49-bc0c-1e4b308327f7",
    "description": "Starts a stack's instances.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instances",
      "item": [
        {
          "id": "52c54256-0cf7-4001-924c-cb9eaf7b093c",
          "name": "assignInstance",
          "request": {
            "url": "http://example.com/api/?Action=AssignInstance?InstanceId=InstanceId&LayerIds=LayerIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assign a registered instance to a layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5e80748-b38d-445e-9d05-4f40aaea44ea"
            }
          ]
        },
        {
          "id": "c1712a33-01f6-4f33-bb54-6c18ea093927",
          "name": "createInstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstance?AgentVersion=AgentVersion&AmiId=AmiId&Architecture=Architecture&AutoScalingType=AutoScalingType&AvailabilityZone=AvailabilityZone&BlockDeviceMappings=BlockDeviceMappings&EbsOptimized=EbsOptimized&Hostname=Hostname&InstallUpdatesOnBoot=InstallUpdatesOnBoot&InstanceType=InstanceType&LayerIds=LayerIds&Os=Os&RootDeviceType=RootDeviceType&SshKeyName=SshKeyName&StackId=StackId&SubnetId=SubnetId&Tenancy=Tenancy&VirtualizationType=VirtualizationType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an instance in a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61739d13-5c60-4f45-83f4-b919ba78838c"
            }
          ]
        },
        {
          "id": "af891880-093d-411a-807a-acd47e8e8501",
          "name": "deleteInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstance?DeleteElasticIp=DeleteElasticIp&DeleteVolumes=DeleteVolumes&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified instance, which terminates the associated Amazon EC2 instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2eaee522-8bf0-4c3b-b682-8668539057e5"
            }
          ]
        },
        {
          "id": "e854e07b-cf4c-46f8-91b1-2329461ee5a9",
          "name": "deregisterInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregister a registered Amazon EC2 or on-premises instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "067e3345-8aa5-4497-b11a-11dcab50604b"
            }
          ]
        },
        {
          "id": "bb7cd7fe-ae9d-4b20-9818-835ad2a2f800",
          "name": "deregisterRdsDbInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterRdsDbInstance?RdsDbInstanceArn=RdsDbInstanceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters an Amazon RDS instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93005f80-2d47-42eb-bc63-be7e322a34e3"
            }
          ]
        },
        {
          "id": "2b39138e-6a0b-4216-a604-d60af84c474b",
          "name": "describeInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstances?InstanceIds=InstanceIds&LayerId=LayerId&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a set of instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dacb37a-0015-492a-8de0-950250c390fb"
            }
          ]
        },
        {
          "id": "1b5127a0-1359-44f4-bbb8-40bc0e2a983b",
          "name": "describeRdsDbInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRdsDbInstances?RdsDbInstanceArns=RdsDbInstanceArns&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Amazon RDS instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8ddb291-c66e-46dc-a5ea-4faad2a68f2b"
            }
          ]
        },
        {
          "id": "5aa1317d-0d91-4fef-8e60-1070f6e9b714",
          "name": "rebootInstance",
          "request": {
            "url": "http://example.com/api/?Action=RebootInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reboots a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8f67b40-eb27-439c-8947-8a70719127ee"
            }
          ]
        },
        {
          "id": "72057164-ca14-48bd-8731-ee030b93eaec",
          "name": "registerInstance",
          "request": {
            "url": "http://example.com/api/?Action=RegisterInstance?Hostname=Hostname&InstanceIdentity=InstanceIdentity&PrivateIp=PrivateIp&PublicIp=PublicIp&RsaPublicKey=RsaPublicKey&RsaPublicKeyFingerprint=RsaPublicKeyFingerprint&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers instances that were created outside of AWS OpsWorks Stacks with a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3caf2e3-50bb-491a-a7bd-cc1d75301ccd"
            }
          ]
        },
        {
          "id": "e9a0bfb2-a07e-4b22-9979-7cb5c8db0abf",
          "name": "registerRdsDbInstance",
          "request": {
            "url": "http://example.com/api/?Action=RegisterRdsDbInstance?DbPassword=DbPassword&DbUser=DbUser&RdsDbInstanceArn=RdsDbInstanceArn&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an Amazon RDS instance with a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21c92977-c76f-4531-bfaf-363c528c0d6f"
            }
          ]
        },
        {
          "id": "5945c617-9d6d-4f83-8958-83501a17e10e",
          "name": "startInstance",
          "request": {
            "url": "http://example.com/api/?Action=StartInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2554e032-34ad-45c8-b6c0-32f6d3d39b88"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "ea442656-0219-42ed-9fc3-85deb065c5a1",
          "name": "assignVolume",
          "request": {
            "url": "http://example.com/api/?Action=AssignVolume?InstanceId=InstanceId&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns one of the stack's registered Amazon EBS volumes to a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a796f0c9-a49b-4a12-a7ee-017500e6cdda"
            }
          ]
        },
        {
          "id": "b46450cd-2fb7-4376-8dc8-5866eb43d68b",
          "name": "deregisterVolume",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterVolume?VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters an Amazon EBS volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04b52e89-1f75-410b-aed3-5e55c6b753b1"
            }
          ]
        },
        {
          "id": "34db9c1e-0652-40ca-86ba-4e5cb95bc4ba",
          "name": "describeVolumes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeVolumes?InstanceId=InstanceId&RaidArrayId=RaidArrayId&StackId=StackId&VolumeIds=VolumeIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes an instance's Amazon EBS volumes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e43b5afb-ae88-444b-9e81-50797c5decbc"
            }
          ]
        },
        {
          "id": "cddb2969-454f-46d2-a6bd-8eaa94ee0c72",
          "name": "registerVolume",
          "request": {
            "url": "http://example.com/api/?Action=RegisterVolume?Ec2VolumeId=Ec2VolumeId&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an Amazon EBS volume with a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e373a3c0-9fed-46bd-a656-e54d6f04f734"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "482b0a52-f9fe-4f70-bd9d-94a87fe587ed",
          "name": "associateElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=AssociateElasticIp?ElasticIp=ElasticIp&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates one of the stack's registered Elastic IP addresses with a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49db2013-aee6-4ec2-94a4-3beb3ed6dbfa"
            }
          ]
        },
        {
          "id": "4c20b0e8-9219-49e2-923a-10dfb5b8abc7",
          "name": "deregisterElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterElasticIp?ElasticIp=ElasticIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters a specified Elastic IP address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94ac51ff-88fa-4217-902a-a0d0b63fb8a1"
            }
          ]
        },
        {
          "id": "f7533f27-bd7d-4956-9229-04a529910ca0",
          "name": "describeElasticIps",
          "request": {
            "url": "http://example.com/api/?Action=DescribeElasticIps?InstanceId=InstanceId&Ips=Ips&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Elastic IPs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2751ad62-cfaf-41a5-bada-a70e525e8841"
            }
          ]
        },
        {
          "id": "4e26b284-d4cd-4fb2-a1c9-de0589f24d84",
          "name": "disassociateElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateElasticIp?ElasticIp=ElasticIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates an Elastic IP address from its instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7dc6ef27-72b2-46cd-b91e-9b8b64ddf794"
            }
          ]
        },
        {
          "id": "327a0b1d-bd25-4966-9838-779bfbc7678d",
          "name": "registerElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=RegisterElasticIp?ElasticIp=ElasticIp&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an Elastic IP address with a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "690e7438-9c90-4e97-8e99-74f24ced178f"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "c08582c2-410d-4fca-8d1b-611c9ce27c43",
          "name": "attachElasticLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=AttachElasticLoadBalancer?ElasticLoadBalancerName=ElasticLoadBalancerName&LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches an Elastic Load Balancing load balancer to a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "866cfced-b2aa-440d-acad-383a62a09bd0"
            }
          ]
        },
        {
          "id": "30d0735d-0d0e-4370-bc48-a01a2893e776",
          "name": "describeElasticLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeElasticLoadBalancers?LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a stack's Elastic Load Balancing instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "497ab7cb-f24b-4d8a-ac9c-d5c1c626a9e4"
            }
          ]
        },
        {
          "id": "fb8705d8-d98e-4c9d-9527-64f9d8ce5674",
          "name": "detachElasticLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=DetachElasticLoadBalancer?ElasticLoadBalancerName=ElasticLoadBalancerName&LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches a specified Elastic Load Balancing instance from its layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42169926-ea07-434a-b144-b1597851aa9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Stacks",
      "item": [
        {
          "id": "de8696c9-c178-4b36-9cf6-70e08d4bdc2f",
          "name": "cloneStack",
          "request": {
            "url": "http://example.com/api/?Action=CloneStack?AgentVersion=AgentVersion&Attributes=Attributes&ChefConfiguration=ChefConfiguration&CloneAppIds=CloneAppIds&ClonePermissions=ClonePermissions&ConfigurationManager=ConfigurationManager&CustomCookbooksSource=CustomCookbooksSource&CustomJson=CustomJson&DefaultAvailabilityZone=DefaultAvailabilityZone&DefaultInstanceProfileArn=DefaultInstanceProfileArn&DefaultOs=DefaultOs&DefaultRootDeviceType=DefaultRootDeviceType&DefaultSshKeyName=DefaultSshKeyName&DefaultSubnetId=DefaultSubnetId&HostnameTheme=HostnameTheme&Name=Name&Region=Region&ServiceRoleArn=ServiceRoleArn&SourceStackId=SourceStackId&UseCustomCookbooks=UseCustomCookbooks&UseOpsworksSecurityGroups=UseOpsworksSecurityGroups&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a clone of a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34f30b4c-b256-4739-8f01-92580375465b"
            }
          ]
        },
        {
          "id": "4fe191df-a52c-4781-9c38-b5589a7b4f07",
          "name": "describeStackProvisioningParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackProvisioningParameters?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a stack's provisioning parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1886947a-af91-4ccf-a496-ca27de07ace2"
            }
          ]
        },
        {
          "id": "18bfa5af-e91c-43fa-827f-861377bda814",
          "name": "describeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?StackIds=StackIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of one or more stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89423c60-45bf-4545-b108-fd34ac6c4c55"
            }
          ]
        },
        {
          "id": "29171345-cf37-4ed2-bddf-3554762122b4",
          "name": "describeStackSummary",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackSummary?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the number of layers and apps in a specified stack, and the number of instances in\n      each state, such as running_setup or online."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "670c9b9d-b445-46db-b80b-51335a2bdb5f"
            }
          ]
        },
        {
          "id": "12ca00eb-b26c-43e4-b87f-c81eca9f5ee0",
          "name": "startStack",
          "request": {
            "url": "http://example.com/api/?Action=StartStack?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a stack's instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe4bff89-acbe-4b44-b5ce-4ffbe7490366"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "99936226-ca58-4d09-b389-1f756ae5fb2b",
          "name": "createApp",
          "request": {
            "url": "http://example.com/api/?Action=CreateApp?AppSource=AppSource&Attributes=Attributes&DataSources=DataSources&Description=Description&Domains=Domains&EnableSsl=EnableSsl&Environment=Environment&Name=Name&Shortname=Shortname&SslConfiguration=SslConfiguration&StackId=StackId&Type=Type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8eafd08-7681-42bf-801d-0c0fd6f723a7"
            }
          ]
        },
        {
          "id": "bbf57e62-ebb1-4136-9722-e907bdff0e24",
          "name": "deleteApp",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApp?AppId=AppId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed08bd6f-9a55-4818-aba6-9bba751a95d8"
            }
          ]
        },
        {
          "id": "14efb2b8-67a9-45bd-9486-b14e8d00cf8e",
          "name": "describeApps",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApps?AppIds=AppIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a specified set of apps."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d4b0bb4-af66-4e3e-a718-0b998c3e9db1"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "5cb7df85-4df9-425d-b3ea-de59dc45aa96",
          "name": "createDeployment",
          "request": {
            "url": "http://example.com/api/?Action=CreateDeployment?AppId=AppId&Command=Command&Comment=Comment&CustomJson=CustomJson&InstanceIds=InstanceIds&LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Runs deployment or stack commands."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2134885-cd62-48e5-9d39-f30e150e8c33"
            }
          ]
        },
        {
          "id": "75d00594-7fbd-4ad2-b406-d0e347786069",
          "name": "createLayer",
          "request": {
            "url": "http://example.com/api/?Action=CreateLayer?Attributes=Attributes&AutoAssignElasticIps=AutoAssignElasticIps&AutoAssignPublicIps=AutoAssignPublicIps&CustomInstanceProfileArn=CustomInstanceProfileArn&CustomJson=CustomJson&CustomRecipes=CustomRecipes&CustomSecurityGroupIds=CustomSecurityGroupIds&EnableAutoHealing=EnableAutoHealing&InstallUpdatesOnBoot=InstallUpdatesOnBoot&LifecycleEventConfiguration=LifecycleEventConfiguration&Name=Name&Packages=Packages&Shortname=Shortname&StackId=StackId&Type=Type&UseEbsOptimizedInstances=UseEbsOptimizedInstances&VolumeConfigurations=VolumeConfigurations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b10dacf8-aac2-419f-b9a9-a14e1de20d86"
            }
          ]
        },
        {
          "id": "07601364-bd27-4508-8e92-0a7d66c99943",
          "name": "createStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?AgentVersion=AgentVersion&Attributes=Attributes&ChefConfiguration=ChefConfiguration&ConfigurationManager=ConfigurationManager&CustomCookbooksSource=CustomCookbooksSource&CustomJson=CustomJson&DefaultAvailabilityZone=DefaultAvailabilityZone&DefaultInstanceProfileArn=DefaultInstanceProfileArn&DefaultOs=DefaultOs&DefaultRootDeviceType=DefaultRootDeviceType&DefaultSshKeyName=DefaultSshKeyName&DefaultSubnetId=DefaultSubnetId&HostnameTheme=HostnameTheme&Name=Name&Region=Region&ServiceRoleArn=ServiceRoleArn&UseCustomCookbooks=UseCustomCookbooks&UseOpsworksSecurityGroups=UseOpsworksSecurityGroups&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e350ffc1-4690-41a5-80f6-4def76a65a75"
            }
          ]
        },
        {
          "id": "a52a95f7-5d3c-498b-b9ed-853edbd4ce76",
          "name": "createUserProfile",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserProfile?AllowSelfManagement=AllowSelfManagement&IamUserArn=IamUserArn&SshPublicKey=SshPublicKey&SshUsername=SshUsername",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new user profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c5df750-6718-4f7b-b857-4ffa6fed4c05"
            }
          ]
        },
        {
          "id": "11525b44-fc72-46ca-8bbe-41ff9cb6d837",
          "name": "deleteLayer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLayer?LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8739fc8-9c7d-40a2-872c-8838b2415920"
            }
          ]
        },
        {
          "id": "88e48614-3a15-409d-847f-8cad0853cf48",
          "name": "deleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d0e7637-9709-43e8-9da3-c2cb0abc5ac7"
            }
          ]
        },
        {
          "id": "30781194-cbae-462f-ad8d-80aa5568d972",
          "name": "deleteUserProfile",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserProfile?IamUserArn=IamUserArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "116cdc5c-012d-4a46-ab34-2fc004abc3c4"
            }
          ]
        },
        {
          "id": "287378cc-69ad-45ae-86c3-ffc55dd5525b",
          "name": "deregisterEcsCluster",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterEcsCluster?EcsClusterArn=EcsClusterArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters a specified Amazon ECS cluster from a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6f9b526-8ee5-480f-91d8-9532486afc8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Agent Versions",
      "item": [
        {
          "id": "76fde3da-6f32-4ad1-a575-5ca6e360db6d",
          "name": "describeAgentVersions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAgentVersions?ConfigurationManager=ConfigurationManager&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available AWS OpsWorks Stacks agent versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f907c5f-1a67-408e-b61a-6306418c56e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Commands",
      "item": [
        {
          "id": "e01d2cb0-bb92-4b74-ac48-368520c65224",
          "name": "describeCommands",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCommands?CommandIds=CommandIds&DeploymentId=DeploymentId&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the results of specified commands."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bb26d49-c6e5-49b7-b451-b8d2e8eff5f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployments",
      "item": [
        {
          "id": "891b69cd-69ca-4a15-b375-3b4ad34def41",
          "name": "describeDeployments",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDeployments?AppId=AppId&DeploymentIds=DeploymentIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a specified set of deployments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58943a17-62d6-4674-92de-a647a68f0123"
            }
          ]
        }
      ]
    },
    {
      "name": "ECS Clusters",
      "item": [
        {
          "id": "a97c4a49-6211-473a-a8c6-89ef4e2d045d",
          "name": "describeEcsClusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEcsClusters?EcsClusterArns=EcsClusterArns&MaxResults=MaxResults&NextToken=NextToken&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Amazon ECS clusters that are registered with a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39ce81e2-8ce2-455a-a286-8c062eadeb55"
            }
          ]
        },
        {
          "id": "191d8318-5e91-4c3e-877c-c8c46b11b83e",
          "name": "registerEcsCluster",
          "request": {
            "url": "http://example.com/api/?Action=RegisterEcsCluster?EcsClusterArn=EcsClusterArn&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a specified Amazon ECS cluster with a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "981a1bfb-496f-402d-8525-b96b309d46d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Layers",
      "item": [
        {
          "id": "c08384d5-61d3-4123-b9a6-e835576d9c8d",
          "name": "describeLayers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLayers?LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of one or more layers in a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5793b59e-1eef-4e86-aa19-2d6d53f7fd1b"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling",
      "item": [
        {
          "id": "46742bbc-ca5e-403e-94c7-364125e6670c",
          "name": "describeLoadBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBasedAutoScaling?LayerIds=LayerIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes load-based auto scaling configurations for specified layers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "491e0d73-e62b-4069-b877-5304869be09f"
            }
          ]
        },
        {
          "id": "d8dea369-9301-4317-9164-dae0112d9164",
          "name": "describeTimeBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTimeBasedAutoScaling?InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes time-based auto scaling configurations for specified instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27b622dc-c49e-4434-9047-2fef5b357c0f"
            }
          ]
        },
        {
          "id": "6018d563-5922-4164-a44a-8c4858dc958c",
          "name": "setLoadBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=SetLoadBasedAutoScaling?DownScaling=DownScaling&Enable=Enable&LayerId=LayerId&UpScaling=UpScaling",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specify the load-based auto scaling configuration for a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8db771fa-8a8b-4a5b-969e-d3a8bcce25e1"
            }
          ]
        },
        {
          "id": "20ea203b-56a2-442d-8364-9f2bc10f7dc2",
          "name": "setTimeBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=SetTimeBasedAutoScaling?AutoScalingSchedule=AutoScalingSchedule&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specify the time-based auto scaling configuration for a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8bc8800-aef3-4f92-be63-87bbd3d69b31"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "acb0f8fc-2aba-4dd7-aac1-bba2d77c8890",
          "name": "describeMyUserProfile",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMyUserProfile?UserProfile=UserProfile",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a user's SSH information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4be344a4-c6e5-450e-9d94-914f53bb3f5c"
            }
          ]
        },
        {
          "id": "044b551d-9a88-4d1b-92cd-c67d755a2acf",
          "name": "describeUserProfiles",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserProfiles?IamUserArns=IamUserArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describe specified users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "043ae909-bac4-4496-b093-9591f388e9e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Permissions",
      "item": [
        {
          "id": "869acb54-63ea-4d1b-ba9c-52784e0b3bc7",
          "name": "describePermissions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePermissions?IamUserArn=IamUserArn&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e78af3f-c548-401f-9119-8010846dd536"
            }
          ]
        },
        {
          "id": "2926f52c-7e01-4670-af7c-ab4c822758d1",
          "name": "setPermission",
          "request": {
            "url": "http://example.com/api/?Action=SetPermission?AllowSsh=AllowSsh&AllowSudo=AllowSudo&IamUserArn=IamUserArn&Level=Level&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies a user's permissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70bdd539-894f-4689-aee3-3c5493f339bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Raid Arrays",
      "item": [
        {
          "id": "ec5e901a-fbc2-49cb-80c4-5693ef12febe",
          "name": "describeRaidArrays",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRaidArrays?InstanceId=InstanceId&RaidArrayIds=RaidArrayIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describe an instance's RAID arrays."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb7e1a4b-d8e5-4f73-afeb-e79e345e79d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Service Errors",
      "item": [
        {
          "id": "d1511b79-6269-45ad-8581-102b9f0299e6",
          "name": "describeServiceErrors",
          "request": {
            "url": "http://example.com/api/?Action=DescribeServiceErrors?InstanceId=InstanceId&ServiceErrorIds=ServiceErrorIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes AWS OpsWorks Stacks service errors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11ad8ba9-ec4c-4dce-a4e2-58044db70f01"
            }
          ]
        }
      ]
    },
    {
      "name": "Host Names",
      "item": [
        {
          "id": "83622b07-4a4b-447d-b2a0-5c2393424ed9",
          "name": "getHostnameSuggestion",
          "request": {
            "url": "http://example.com/api/?Action=GetHostnameSuggestion?LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a generated host name for the specified layer, based on the current host name theme."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31b33205-ef26-4b0c-9e8c-3deb98e99af1"
            }
          ]
        }
      ]
    },
    {
      "name": "Access",
      "item": [
        {
          "id": "45f386fa-c789-422f-a034-2dd0a483fe46",
          "name": "grantAccess",
          "request": {
            "url": "http://example.com/api/?Action=GrantAccess?InstanceId=InstanceId&ValidForInMinutes=ValidForInMinutes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis action can be used only with Windows stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26be5976-cb99-4bc1-a9a8-0c1b0627b57a"
            }
          ]
        }
      ]
    }
  ]
}