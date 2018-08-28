{
  "info": {
    "name": "AWS Directory Service API Disable Radius",
    "_postman_id": "94a80173-86d2-43d9-9b3c-05bcc2db9023",
    "description": "Disables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "a2e9ced6-329b-4500-9d49-bd67c7c0df7e",
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
              "id": "af398037-c7c6-4e2e-8dad-8955ea0c3abf"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "1421094c-dbc1-4e98-93b8-b97500b36e14",
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
              "id": "0782839c-708a-46d4-8926-c1895f23e497"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "ab55813d-142c-4c3e-99e3-3e31c5a36fd2",
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
              "id": "ad0b5a0b-ff03-44a3-a53d-1ef2ffbb7642"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "0291b018-edfc-4bc6-945c-88dc72ef9641",
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
              "id": "075954da-dab0-400c-9639-cdd9efd4ec0a"
            }
          ]
        },
        {
          "id": "fc82b359-b427-403e-af2b-b736ae78b743",
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
              "id": "0a3db419-34d8-4f88-9f9a-74eca0bf2f91"
            }
          ]
        },
        {
          "id": "9934c6ae-9fd4-40af-96e8-e455f1a5b56a",
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
              "id": "8269da7e-f565-4df7-889b-bf061085869c"
            }
          ]
        },
        {
          "id": "2ebbf886-1be3-48d8-9b22-dac46d3af467",
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
              "id": "ceaf4bae-fb0e-4192-a872-dccd185daff0"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "39066377-a7c2-4da7-9dc8-493f52db5e77",
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
              "id": "b39314f9-e1f6-4bff-964d-083b61ba9781"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "7222b8ab-74b8-4a4c-8b66-4d6d7e45d90c",
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
              "id": "0c346d5b-0616-458a-aa3a-57deb01db0cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "93ca2035-37f3-4cc3-9a95-8875aebd31b2",
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
              "id": "61b60a2e-65d3-4d82-bb11-c1cc8c51949f"
            }
          ]
        },
        {
          "id": "efd823e1-20c1-4c58-8f44-d6aae9ba58ab",
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
              "id": "d9b37aeb-1401-4878-bb25-b88a0853c104"
            }
          ]
        },
        {
          "id": "672b7982-2472-465c-8d3c-9034b17750a9",
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
              "id": "73795316-6455-4d6b-a8ef-39613545bd54"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "684a44cf-f84b-4075-a70f-5434d2e114ad",
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
              "id": "e1a9569b-66bc-4cfe-beb4-17f6c93badbf"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "0a0476bc-64af-428a-a8c4-0690c8eeb7a4",
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
              "id": "3119bf99-a827-47e1-9eb6-ac2133db2472"
            }
          ]
        }
      ]
    },
    {
      "name": "Trust",
      "item": [
        {
          "id": "9765de30-46e3-4654-9820-d3a85ad60a2d",
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
              "id": "783220de-5812-4b0a-906e-9907611c8b22"
            }
          ]
        },
        {
          "id": "6099dc66-edd6-41d4-91b3-489f295e6efb",
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
              "id": "3fc89e81-0dee-40bb-96e9-5c984d8150db"
            }
          ]
        },
        {
          "id": "0956133c-d7cd-4006-a7de-2f4bc0913a09",
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
              "id": "74d4ef7b-e0fe-4d40-b748-5364e4df31a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "6c4badd4-6d63-4822-90cf-4604d34ba5c2",
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
              "id": "a358c1fa-1570-4cd4-8f98-4a7ed4dd918a"
            }
          ]
        },
        {
          "id": "70ccf3a1-7c47-4ae8-9f36-f5140ae529a9",
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
              "id": "4051307f-3e1c-4392-87a2-9a59ee102b1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "125c0fa1-9c75-41ef-96ed-f92b8c1b35e5",
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
              "id": "63760599-6f13-444d-ae95-30d350d15fe6"
            }
          ]
        },
        {
          "id": "d0b8bf32-f8da-46e3-9335-9e8192e6cd72",
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
              "id": "f709db25-8493-45e4-91eb-c4d88d513afb"
            }
          ]
        }
      ]
    },
    {
      "name": "Radius",
      "item": [
        {
          "id": "fa7b6276-8a90-40e8-b25a-6118f19fa669",
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
              "id": "09f5bc80-ab64-44be-93fe-e48ef3a1ebcd"
            }
          ]
        }
      ]
    }
  ]
}