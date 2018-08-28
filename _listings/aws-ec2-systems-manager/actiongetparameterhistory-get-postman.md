{
  "info": {
    "name": "Amazon EC2 Systems Manager API Get Parameter History",
    "_postman_id": "3524e831-655b-4212-854f-8de971bd91b2",
    "description": "Query a list of all parameters used by the AWS account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "5aa53adb-f4b4-4777-a6e6-39e38473875c",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac7dff60-4c82-4efa-993c-7debdae61f11"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "a79817fe-2977-402f-91fa-026b02c031c0",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c13bf9f3-cc33-44df-aa47-3abe9a1c3825"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "468cc769-7d99-4514-b252-62f358591d58",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2aff707-ddb0-43ff-9571-53e5da51a7f6"
            }
          ]
        },
        {
          "id": "69e66222-0c05-4251-a9c4-a6f2dc85eb9e",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02bbce67-16e4-4e1f-96b1-7472eaa1cdc3"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "649f8667-bf64-4987-ac82-85aa874ba4ac",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7682825-1862-4de6-866a-3f8da0f70fb8"
            }
          ]
        },
        {
          "id": "d1562d4b-9c0f-46e6-bc45-23916f4d4a57",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5941eb75-91cd-43e9-9c34-25c5af877d30"
            }
          ]
        },
        {
          "id": "269bce7c-18fb-47d5-ab6a-014537cb9f3b",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cf2d529-6206-4cbc-b32b-69c049110c79"
            }
          ]
        },
        {
          "id": "dc38f0c8-ffaf-457f-8099-9d943ae85ec4",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73a4cae1-8c4b-42c3-a5e2-215480ce63fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "feea640f-cd0b-4440-abf3-94d8c2d45bd4",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e8b0d0c-8dbc-4846-9f7e-cc31111a7be8"
            }
          ]
        },
        {
          "id": "89c019e3-777c-44da-9f5e-4607019613e8",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "765ca214-ca91-4212-9b15-a272aefbb565"
            }
          ]
        },
        {
          "id": "fe6f6657-0632-4d0e-be86-cd79d89c88ce",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0c64302-6c4c-499c-b90a-e7828e60b7c6"
            }
          ]
        },
        {
          "id": "885ebe2f-8262-4b64-ab57-d38eeb0af883",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9cfc694-b61c-40dd-9db7-b7555b45a676"
            }
          ]
        },
        {
          "id": "fa4bc58e-ae0e-439b-a963-152742ef1248",
          "name": "getDocument",
          "request": {
            "url": "http://example.com/api/?Action=GetDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the contents of the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c61b880-dfb6-4264-8cd7-4be5315092b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "53d8133e-d8d7-4606-aa90-927413e2c469",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca3b4c93-7f3a-4e5c-9d79-8426360e6c91"
            }
          ]
        },
        {
          "id": "92935e7e-3d6e-42b4-8fbe-046c6629da14",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "493dff21-54a7-48cc-b98d-98426aa1dcda"
            }
          ]
        },
        {
          "id": "c85fff85-fb58-48c0-88d7-31d88da2b985",
          "name": "describeMaintenanceWindowExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a Maintenance Window (meaning, information about when the\n   Maintenance Window was scheduled to be active and information about tasks registered and run with\n   the Maintenance Window)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "259c2b74-c260-41ac-a2e7-0835d39a9963"
            }
          ]
        },
        {
          "id": "f1e44aea-272d-4e98-84cf-af8b17d3c56d",
          "name": "describeMaintenanceWindowExecutionTaskInvocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTaskInvocations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the individual task executions (one per target) for a particular task executed\n   as part of a Maintenance Window execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59fd9de2-09f6-44c8-b091-b9c88593798d"
            }
          ]
        },
        {
          "id": "39da48bd-3be7-4239-9777-3fba77b961a9",
          "name": "describeMaintenanceWindowExecutionTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given Maintenance Window execution, lists the tasks that were executed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bccded3-77de-4941-a61f-a2e3204c62c4"
            }
          ]
        },
        {
          "id": "860264f5-bc84-4fcf-8b4e-17d204c454be",
          "name": "describeMaintenanceWindows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindows?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the Maintenance Windows in an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15ee77f5-aae8-4786-a8ba-46cd98e3d09e"
            }
          ]
        },
        {
          "id": "4dabee17-aafc-4b83-b02d-d610081b075f",
          "name": "describeMaintenanceWindowTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTargets?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the targets registered with the Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f418c7eb-f94f-4d1f-b41d-032a0e1cdd83"
            }
          ]
        },
        {
          "id": "0303a51a-8540-4bca-a488-8db9f2aa0086",
          "name": "describeMaintenanceWindowTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tasks in a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed3f6f9a-8975-4321-a182-fe5b79aa16ce"
            }
          ]
        },
        {
          "id": "d5bc4b0d-5fd8-4414-9ad1-5efccba5d41a",
          "name": "getMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cffa2a18-c689-4477-90ef-8976cd23e3d9"
            }
          ]
        },
        {
          "id": "a2aba6be-38ec-4e1e-a04c-9a0f7f03ffb1",
          "name": "getMaintenanceWindowExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecution?WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a4e041c-82f2-4791-b857-7ddb83acc35f"
            }
          ]
        },
        {
          "id": "2d11a0d2-54eb-4be9-a10c-6b3aa5b09b25",
          "name": "getMaintenanceWindowExecutionTask",
          "request": {
            "url": "http://example.com/api/?Action=GetMaintenanceWindowExecutionTask?TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details about a specific task executed as part of a Maintenance Window\n   execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c20cb88d-ab39-431e-8c12-37cfff069136"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "e72488f9-bbd4-4ee7-8eef-12d354d3b834",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d79a03bb-5c7d-4ae1-b9f1-23a5f881e0c1"
            }
          ]
        },
        {
          "id": "804cdf33-8e0e-4ad9-9c48-c6a3b03268f7",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc04b122-df1f-403f-9032-5def03cc8401"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "b4027dd7-396a-4140-ac09-97550ff883b1",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02af28e7-8f5e-4542-9ba4-d0a89b074532"
            }
          ]
        },
        {
          "id": "a14f112f-dc79-44fb-a3cf-a00362d14510",
          "name": "getParameterHistory",
          "request": {
            "url": "http://example.com/api/?Action=GetParameterHistory?MaxResults=MaxResults&Name=Name&NextToken=NextToken&WithDecryption=WithDecryption",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query a list of all parameters used by the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc56bde6-136e-41c2-994b-c7e41fb00595"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "36fa1cd0-cf53-401e-8ace-3fa2f2dbc125",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "750cb8bc-22c4-462e-b9ae-21132999ff65"
            }
          ]
        },
        {
          "id": "8d5f5b49-0eae-49a0-96c6-414ea515f284",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d48b956d-19fd-47dc-8982-b2b87c138a75"
            }
          ]
        },
        {
          "id": "58d5bd8d-8620-43d5-957e-ce28e605b4d0",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea766ea0-d3d8-4a51-afdb-baf51e910db4"
            }
          ]
        },
        {
          "id": "66bb8b10-7217-4014-b3f7-eeadba2b48c8",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b463789f-078c-4994-aeea-b71bb4799edb"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "6b120a05-0687-4fef-962d-00fa363988c1",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfa124d6-83c3-4c6c-9d66-8b5726bfacd1"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "cf01aba8-2850-4c56-971a-6c6fa4ee7b81",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "625fc985-bcee-48ba-bf1a-4651bac16f88"
            }
          ]
        },
        {
          "id": "bb61cdde-2106-4b1c-9e9e-dbd990140d9a",
          "name": "getAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detailed information about a particular Automation execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcce7c6f-1923-4faf-a4e8-ce45502980a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "8f62812d-f773-4a18-98a2-671270ca2ee0",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eaf61354-59a1-4374-8e84-0ab2a4d1998c"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "d22c0a42-68d5-4fc8-a63a-7ade6defc18e",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ede8342d-6d15-42f4-a81c-1f2629035461"
            }
          ]
        },
        {
          "id": "dd7bb19e-cda5-491c-8e7c-378ec4267e8b",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dc8526e-b1b4-4e8d-8923-dfd437d5ecf0"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "243ee1b5-e932-4502-8f7f-93c690f71c3b",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02329472-4f63-4669-94a9-3cde5d543675"
            }
          ]
        },
        {
          "id": "8780ce4b-2dc1-4728-be03-ab590acd5ded",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b9ead01-55b8-4163-8751-8a8815d84dcf"
            }
          ]
        },
        {
          "id": "78fb07af-71c1-45a2-bdb4-39c5745854e6",
          "name": "describeInstancePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatches?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the patches on the specified instance and their state relative to the patch baseline being used for the instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0aae68c-1e9c-490a-bb68-2ec369c98407"
            }
          ]
        },
        {
          "id": "7a77ac0c-58e1-4e13-a54d-1ad5aaa53376",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c2efae3-ad74-4fbe-a9e0-7008643bb07f"
            }
          ]
        },
        {
          "id": "464bf554-7e25-4776-932b-ebb3e322ab7e",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cc0a5f6-e979-4a55-9d53-79119036cb1e"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "305da23c-58d4-4f67-bb5c-38c622c29688",
          "name": "describeParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeParameters?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ba7e1e7-4306-4dc4-8a71-edb5640f3156"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "ab7c38c5-042e-45c4-bb2a-b7765f201b6c",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67f55236-82c0-496b-997b-18dc528e771a"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "8485f0de-d77b-4e52-ae1a-7b7019f8c5c0",
          "name": "describePatchGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroups?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patch groups that have been registered with patch baselines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88b3ef30-baa1-4d7e-b1a8-c0f9f62e6a88"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "eed436ab-3b84-45b3-a9da-da4f0168155c",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b16f8fd5-78a9-414c-81af-fb9bcda0e6c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "529b72d7-15aa-4b2a-b44c-cd673aac5602",
          "name": "getCommandInvocation",
          "request": {
            "url": "http://example.com/api/?Action=GetCommandInvocation?CommandId=CommandId&InstanceId=InstanceId&PluginName=PluginName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information about command execution for an invocation or plugin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3cbb7e6-b3d7-4d12-b6c2-04ab10786d5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "909cc5f4-c15e-405c-be67-8008e29933ff",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5e29030-fac7-4c5b-a799-52021a74f37f"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "64c2debc-2196-4d33-8d7d-01093fd347d3",
          "name": "getDeployablePatchSnapshotForInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetDeployablePatchSnapshotForInstance?InstanceId=InstanceId&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current snapshot for the patch baseline the instance uses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a2c7699-e2b8-4017-a64f-6a619129a5fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Inventory",
      "item": [
        {
          "id": "33d4b7d7-2817-4cf8-9cc7-d9769920971d",
          "name": "getInventory",
          "request": {
            "url": "http://example.com/api/?Action=GetInventory?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&ResultAttributes=ResultAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query inventory information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40d5257b-0a03-4560-b4da-cf32a8e9efce"
            }
          ]
        },
        {
          "id": "e7029a5f-d192-45b4-ab86-4be3909d8538",
          "name": "getInventorySchema",
          "request": {
            "url": "http://example.com/api/?Action=GetInventorySchema?MaxResults=MaxResults&NextToken=NextToken&TypeName=TypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of inventory type names for the account, or return a list of attribute\n   names for a specific Inventory item type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0daa9700-cb49-4999-b5f2-1a28fad916ee"
            }
          ]
        }
      ]
    }
  ]
}