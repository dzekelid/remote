{
  "info": {
    "name": "AWS Directory Service API Enable Radius",
    "_postman_id": "a31dc315-b631-4eaa-b77a-7fc85f871f97",
    "description": "Enables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "6a479a72-2c9f-4c5d-96c1-f092bf95ef80",
          "name": "addIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=AddIpRoutes?DirectoryId=DirectoryId&IpRoutes=IpRoutes&UpdateSecurityGroupForDirectoryControllers=UpdateSecurityGroupForDirectoryControllers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If the DNS server for your on-premises domain uses a publicly addressable IP address, you must add a CIDR address block to correctly route traffic to and from your Microsoft AD on Amazon Web Services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bb2c3ae-245c-455b-8bf4-f99a6f42603e"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "45768a55-7491-4585-b247-a491549e13b6",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e42507c9-3a4d-4fe6-a054-7c05b9fe9a30"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "144bc137-d88f-444d-84b8-a4637e22931f",
          "name": "cancelSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=CancelSchemaExtension?DirectoryId=DirectoryId&SchemaExtensionId=SchemaExtensionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an in-progress schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "976e82ff-51dc-44b8-b50d-664d38dd6b0c"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "f9991b43-b604-4c88-a04a-2f8794998b9a",
          "name": "connectDirectory",
          "request": {
            "url": "http://example.com/api/?Action=ConnectDirectory?ConnectSettings=ConnectSettings&Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AD Connector to connect to an on-premises directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74c9fd96-b508-487b-b3e1-f2c4849b880a"
            }
          ]
        },
        {
          "id": "6977a59b-9a48-4c6c-af25-a80c127b4c32",
          "name": "createDirectory",
          "request": {
            "url": "http://example.com/api/?Action=CreateDirectory?Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Simple AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49ea8ff4-770f-44d6-b954-a59e3bdb1b7a"
            }
          ]
        },
        {
          "id": "9609fe1e-c88d-439a-b712-126be56e690c",
          "name": "deleteDirectory",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDirectory?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Directory Service directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d178d525-dda5-4a33-b456-0e3f53defd77"
            }
          ]
        },
        {
          "id": "87312b68-0768-4a3a-b82f-8380342d279a",
          "name": "describeDirectories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDirectories?DirectoryIds=DirectoryIds&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directories that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0129b4b-9211-421c-9ba0-1f95176f32ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "4a610b2a-12ba-449d-90d9-9b8b7c36224a",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?Alias=Alias&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for a directory and assigns the alias to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10dbec9f-2534-4bc8-afbb-32254c525eb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "cc66098e-fb88-405c-8836-1df8a983e696",
          "name": "createComputer",
          "request": {
            "url": "http://example.com/api/?Action=CreateComputer?ComputerAttributes=ComputerAttributes&ComputerName=ComputerName&DirectoryId=DirectoryId&OrganizationalUnitDistinguishedName=OrganizationalUnitDistinguishedName&Password=Password",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a computer account in the specified directory, and joins the computer to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e83a191c-afad-4524-b0bc-17e99cf0b70a"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "15a5fbf7-0872-4b71-9c34-99ba13e808e2",
          "name": "createConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=CreateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a conditional forwarder associated with your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb08f113-4c57-4e03-bf8b-f6e43cfbbe61"
            }
          ]
        },
        {
          "id": "15f66a1b-e1b0-425e-9175-f50989f9d05e",
          "name": "deleteConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConditionalForwarder?DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1007569e-65e2-4277-b408-b0a7e506a9e1"
            }
          ]
        },
        {
          "id": "18ab0674-8dbe-4eb7-9ca1-53dcf976ec0e",
          "name": "describeConditionalForwarders",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConditionalForwarders?DirectoryId=DirectoryId&RemoteDomainNames=RemoteDomainNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the conditional forwarders for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d6300dc-1a00-4e1a-841c-200b53dac15f"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "5b03fcac-993b-4326-9f17-3df79833759b",
          "name": "createMicrosoftAD",
          "request": {
            "url": "http://example.com/api/?Action=CreateMicrosoftAD?Description=Description&Name=Name&Password=Password&ShortName=ShortName&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Microsoft AD in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "392ae8eb-04c6-40ed-b661-20f534a79265"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "edc8b651-80cb-43cf-b5bd-c9cad0f5f77a",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?DirectoryId=DirectoryId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a Simple AD or Microsoft AD directory in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3361b19-91f0-44db-a803-7bd1bfb54038"
            }
          ]
        }
      ]
    },
    {
      "name": "Trust",
      "item": [
        {
          "id": "9c2c454b-008b-4c97-af3d-87ec1d1c8e1e",
          "name": "createTrust",
          "request": {
            "url": "http://example.com/api/?Action=CreateTrust?ConditionalForwarderIpAddrs=ConditionalForwarderIpAddrs&DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName&TrustDirection=TrustDirection&TrustPassword=TrustPassword&TrustType=TrustType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AWS Directory Service for Microsoft Active Directory allows you to configure trust relationships."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bd102ad-20d5-498f-ba24-26e27c3fdb99"
            }
          ]
        },
        {
          "id": "10c60a8d-41fc-4a3d-89b8-300e1b0f862a",
          "name": "deleteTrust",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTrust?DeleteAssociatedConditionalForwarder=DeleteAssociatedConditionalForwarder&TrustId=TrustId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing trust relationship between your Microsoft AD in the AWS cloud and an external domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27c78dcb-5913-4ce7-a1c7-f5ad1d85ec21"
            }
          ]
        },
        {
          "id": "4ce9898a-de41-41c5-8b44-86402131f9b7",
          "name": "describeTrusts",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTrusts?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&TrustIds=TrustIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the trust relationships for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c680e8d-78d3-48ac-b2aa-baae698c1475"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "d8805032-fbd6-488a-9161-b8ffa7103491",
          "name": "deleteSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fe52797-5092-4cec-ace7-a46864cd0dde"
            }
          ]
        },
        {
          "id": "a165df6e-9df9-4459-bc9b-c96a8bd11596",
          "name": "describeSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshots?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&SnapshotIds=SnapshotIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directory snapshots that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4c2a9ef-d450-4838-b1ed-ade1281b4a56"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "a55f3d5f-e091-495b-937b-0f6434e05b8a",
          "name": "deregisterEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified directory as a publisher to the specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bd460ac-a601-4f2b-889c-50b17318e119"
            }
          ]
        },
        {
          "id": "a0f369a4-4c24-4486-a3fc-112a1bd59d74",
          "name": "describeEventTopics",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventTopics?DirectoryId=DirectoryId&TopicNames=TopicNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about which SNS topics receive status messages from the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0abb9e6-dac7-49b8-9e6b-34c3f20c3e4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Radius",
      "item": [
        {
          "id": "71218379-73a4-47a3-ab84-dfcb9005687b",
          "name": "disableRadius",
          "request": {
            "url": "http://example.com/api/?Action=DisableRadius?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "788435dd-dab5-4239-9cf9-5c5325c5f4f4"
            }
          ]
        },
        {
          "id": "5b35de76-45e2-4d1d-a6fe-95d482454e8f",
          "name": "enableRadius",
          "request": {
            "url": "http://example.com/api/?Action=EnableRadius?DirectoryId=DirectoryId&RadiusSettings=RadiusSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "495c5c10-392c-4c6d-8835-ca4a7d6bb008"
            }
          ]
        }
      ]
    },
    {
      "name": "SSO",
      "item": [
        {
          "id": "5debe2bd-962d-4510-8ece-c7766d1bc046",
          "name": "disableSso",
          "request": {
            "url": "http://example.com/api/?Action=DisableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables single-sign on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdd99c9a-22c1-4fd0-8d32-ad864afdb62b"
            }
          ]
        }
      ]
    }
  ]
}