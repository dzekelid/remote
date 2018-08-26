{
  "info": {
    "name": "AWS Directory Service API Update Radius",
    "_postman_id": "505c3a2c-4833-43c8-89e1-e592cb62511a",
    "description": "Updates the Remote Authentication Dial In User Service (RADIUS) server information for an AD Connector directory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "0ae71233-8244-4bf2-9b1d-4dc1518e61b2",
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
              "id": "46684108-0d6c-4086-aa74-7ca55d858c75"
            }
          ]
        },
        {
          "id": "ca1d1499-b80c-4dba-b115-1d740c314578",
          "name": "listIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=ListIpRoutes?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the address blocks that you have added to a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbfbbb67-eb53-4c0f-b8bb-426ec6165a42"
            }
          ]
        },
        {
          "id": "e137523c-3cc9-4ca1-8a5b-3231a29e5b49",
          "name": "removeIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=RemoveIpRoutes?CidrIps=CidrIps&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes IP address blocks from a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7897edb1-fa44-45cb-9a4a-e11478b5bc1d"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "4807c967-fee7-42ca-b38b-5f1dbd526ad4",
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
              "id": "c765dae1-5ad9-4de2-9ae3-9fbf0f3f5391"
            }
          ]
        },
        {
          "id": "92d74d9c-9264-4e32-b398-dabd146f5125",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Limit=Limit&NextToken=NextToken&ResourceId=ResourceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "979eeedf-6c3a-47fe-9aed-d89a88079a45"
            }
          ]
        },
        {
          "id": "4babc552-836a-4349-855e-e5448aaa7705",
          "name": "removeTagsFromResource",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTagsFromResource?ResourceId=ResourceId&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e202cde-0b16-426b-b1e4-49a93e2fb21c"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "f3f1a872-1ea5-4729-ab9f-82934b5225b6",
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
              "id": "b506c3ea-73b3-41e5-9ce5-8bc25604149e"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "6ff73659-7edb-469b-a4ed-e23d1488ec44",
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
              "id": "4fb56a4f-5c1b-47be-bec9-723f6cbe3640"
            }
          ]
        },
        {
          "id": "b788947c-6934-40f1-95fe-061dc1dfdeb1",
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
              "id": "7ae62943-e746-436d-8aa5-7088072f2747"
            }
          ]
        },
        {
          "id": "2cd5aa4c-8ae1-4481-a4b6-4316f838274f",
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
              "id": "a1941f80-809a-4ba9-a2d3-af2632b2e106"
            }
          ]
        },
        {
          "id": "700357d8-aae1-46f1-b393-958c36246122",
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
              "id": "2fb9a659-7692-4525-94af-15b78b728c01"
            }
          ]
        },
        {
          "id": "cd909c87-eb58-437f-a9df-fc2553514ae9",
          "name": "getDirectoryLimits",
          "request": {
            "url": "http://example.com/api/?Action=GetDirectoryLimits?DirectoryLimits=DirectoryLimits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains directory limit information for the current region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30ba3ed8-66d7-4908-a5e4-c701b4763fe8"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "5b7a48b6-b98f-4701-8d0c-cec8c201f6ac",
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
              "id": "2aea4a21-7dde-4748-8c58-7db31699ef13"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "25c9d785-a88d-4e18-894b-fe0b3f74d1e5",
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
              "id": "beb1ae59-8e30-4fd3-a216-7e95e9dda4f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "a91fb054-cb19-42e7-9907-928e8a97cebb",
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
              "id": "0bef7d66-9dec-446b-8bad-e74f9833894e"
            }
          ]
        },
        {
          "id": "1268c23d-6288-40d2-9638-dadbc277ce90",
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
              "id": "67703367-dba0-44ee-be14-f1dfa9aea361"
            }
          ]
        },
        {
          "id": "1f26d6ae-c99e-4a55-82ba-14efbd665277",
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
              "id": "df50bf6a-9bb9-4d53-bbce-1b7010ae808b"
            }
          ]
        },
        {
          "id": "2530bf9f-5ddd-42db-9ec5-4ef33d97abde",
          "name": "updateConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=UpdateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7fc7241-9870-4b64-a58b-eaf9fa3bc667"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "3d8832fe-d863-43c6-ad79-584993610152",
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
              "id": "15e17823-af72-4cc9-ab26-17d7379a1bb7"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "3eae5104-96f9-4bdb-99d3-4c3ad7a910fd",
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
              "id": "4f3e83b8-bcb1-4885-9405-b147483aa8aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Trust",
      "item": [
        {
          "id": "2bd5940b-7a0a-4dcc-83dd-4f3198360836",
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
              "id": "5aa3461b-e7cf-41a6-b736-09e310078906"
            }
          ]
        },
        {
          "id": "b6318f0f-db7d-48b4-8b9d-ff73c9f3ad49",
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
              "id": "0c908076-93f6-40be-9709-4a1b2a669332"
            }
          ]
        },
        {
          "id": "61659c3c-82a1-4ea3-835f-dfff845ad41a",
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
              "id": "493a886b-56c2-4a9f-b06f-c2541ab3a4cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "fe64de0b-7d40-4510-b3b9-bf5db01be28b",
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
              "id": "00a9bc81-042b-41ce-9923-81af3eea9088"
            }
          ]
        },
        {
          "id": "e30ceed5-899c-44a5-a8c8-89380bf8f90b",
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
              "id": "6cd22b31-32da-4e7d-b255-21b06094cda9"
            }
          ]
        },
        {
          "id": "f29e8968-91c0-4d79-bc65-1df62d5d5452",
          "name": "getSnapshotLimits",
          "request": {
            "url": "http://example.com/api/?Action=GetSnapshotLimits?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains the manual snapshot limits for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87eb7eaa-5b21-4718-a35a-f3192c7f2e17"
            }
          ]
        },
        {
          "id": "53e84607-cda5-430f-bc3d-6fe9570b186a",
          "name": "restoreFromSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=RestoreFromSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Restores a directory using an existing directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b243ff3-0a02-4698-b858-82554d581619"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "957e3cf9-3c9f-441a-b34b-00f8b73c32f5",
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
              "id": "d2f76ee5-42a8-47de-9739-c80e8ca5dc08"
            }
          ]
        },
        {
          "id": "9e4758ba-a9d3-46ad-b522-53561c769918",
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
              "id": "220dba0d-56c9-4a57-9109-9345a97de368"
            }
          ]
        },
        {
          "id": "1ac7c6a7-a810-4e2b-9b95-9a85b3f4cf2a",
          "name": "registerEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=RegisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a directory with an SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c7dd8f3-62a7-4388-b311-6f8d05837e79"
            }
          ]
        }
      ]
    },
    {
      "name": "Radius",
      "item": [
        {
          "id": "e93a1343-5d11-48e6-8188-84aa11ee8328",
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
              "id": "85b8c832-0a97-43a2-91a3-37e99c7f8703"
            }
          ]
        },
        {
          "id": "0720ff51-2fb0-43a5-9f44-4f99b92e666d",
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
              "id": "f97a9c57-54f6-4e46-a640-ab4e4882ce5f"
            }
          ]
        },
        {
          "id": "69ace9ef-3a24-417a-88d3-692a24d34f8c",
          "name": "updateRadius",
          "request": {
            "url": "http://example.com/api/?Action=UpdateRadius?DirectoryId=DirectoryId&RadiusSettings=RadiusSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the Remote Authentication Dial In User Service (RADIUS) server information for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a352838-2ad0-4905-a4ca-d77eb38410e5"
            }
          ]
        }
      ]
    },
    {
      "name": "SSO",
      "item": [
        {
          "id": "b6c02d91-2516-47b2-9538-d2904a33b920",
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
              "id": "4c906e73-4fe6-4ebb-9e68-92e28f447c26"
            }
          ]
        },
        {
          "id": "77ede0b9-9bbe-4f60-9c57-09208a3c8543",
          "name": "enableSso",
          "request": {
            "url": "http://example.com/api/?Action=EnableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables single sign-on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b064c54d-f1c0-4e71-9022-d610030a4271"
            }
          ]
        }
      ]
    },
    {
      "name": "Schema Extension",
      "item": [
        {
          "id": "fe2ffc5c-be75-444c-a6e8-4aa76467563b",
          "name": "listSchemaExtensions",
          "request": {
            "url": "http://example.com/api/?Action=ListSchemaExtensions?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all schema extensions applied to a Microsoft AD Directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ab15110-87a4-4fbd-851e-ce4c69366da2"
            }
          ]
        },
        {
          "id": "4da838d9-7881-49e4-96c2-3bc9900590e2",
          "name": "startSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=StartSchemaExtension?CreateSnapshotBeforeSchemaExtension=CreateSnapshotBeforeSchemaExtension&Description=Description&DirectoryId=DirectoryId&LdifContent=LdifContent",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b418d90-2436-411f-9200-bdd42c275ec4"
            }
          ]
        }
      ]
    }
  ]
}