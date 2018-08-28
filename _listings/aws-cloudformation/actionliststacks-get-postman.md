{
  "info": {
    "name": "AWS CloudFormation API List Stacks",
    "_postman_id": "fc269605-2315-48ca-b296-b5af8cd44775",
    "description": "Returns the summary information for stacks whose status matches the specified StackStatusFilter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "dc978a7e-2091-494f-8835-58b8348eb6cf",
          "name": "cancelUpdateStack",
          "request": {
            "url": "http://example.com/api/?Action=CancelUpdateStack?StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an update on the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "441ea1c0-4006-4376-beb6-a68811a667f3"
            }
          ]
        },
        {
          "id": "5994b805-99e3-45a3-9879-e22d732ee597",
          "name": "createStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?Capabilities.member.N=Capabilities.member.N&DisableRollback=DisableRollback&NotificationARNs.member.N=NotificationARNs.member.N&OnFailure=OnFailure&Parameters.member.N=Parameters.member.N&ResourceTypes.member.N=ResourceTypes.member.N&RoleARN=RoleARN&StackName=StackName&StackPolicyBody=StackPolicyBody&StackPolicyURL=StackPolicyURL&Tags.member.N=Tags.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL&TimeoutInMinutes=TimeoutInMinutes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a stack as specified in the template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2942de03-4c8a-4942-8bdd-f3b7ee11316c"
            }
          ]
        },
        {
          "id": "8c179b8c-4be0-458c-b9fc-b1d0b121874b",
          "name": "deleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?RetainResources.member.N=RetainResources.member.N&RoleARN=RoleARN&StackName=StackName",
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
              "id": "e2f5c2d4-f9b6-43e0-b0d7-d7b359fb3834"
            }
          ]
        },
        {
          "id": "6ba80dd6-029e-4b2c-a531-3dc5faa3cdd3",
          "name": "describeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the description for the specified stack; if no stack name was specified, then it returns the description for all the stacks created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5aa9f9a8-2a4e-42d2-b31a-a05f58eeef7b"
            }
          ]
        },
        {
          "id": "e77b2363-fd02-4055-afca-f2e1f3294659",
          "name": "listStacks",
          "request": {
            "url": "http://example.com/api/?Action=ListStacks?NextToken=NextToken&StackStatusFilter.member.N=StackStatusFilter.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the summary information for stacks whose status matches the specified StackStatusFilter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3da76c19-a379-4e33-930b-b50183805789"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "3fdec817-f2cd-44bc-830d-2807e5c4867a",
          "name": "continueUpdateRollback",
          "request": {
            "url": "http://example.com/api/?Action=ContinueUpdateRollback?ResourcesToSkip.member.N=ResourcesToSkip.member.N&RoleARN=RoleARN&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back\n         to the UPDATE_ROLLBACK_COMPLETE state."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb54b093-cd34-4185-b1b2-b08d6e32048c"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Sets",
      "item": [
        {
          "id": "0db528fb-e5d8-46c1-a32a-c03e680443e9",
          "name": "createChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateChangeSet?Capabilities.member.N=Capabilities.member.N&ChangeSetName=ChangeSetName&ChangeSetType=ChangeSetType&ClientToken=ClientToken&Description=Description&NotificationARNs.member.N=NotificationARNs.member.N&Parameters.member.N=Parameters.member.N&ResourceTypes.member.N=ResourceTypes.member.N&RoleARN=RoleARN&StackName=StackName&Tags.member.N=Tags.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL&UsePreviousTemplate=UsePreviousTemplate",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a list of changes for a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3822c9e6-f9cf-4137-aeb3-e5adaa8bb334"
            }
          ]
        },
        {
          "id": "645f7521-3f36-433b-86b1-de22bb013d69",
          "name": "deleteChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteChangeSet?ChangeSetName=ChangeSetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified change set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f848f33c-c2d8-4a8c-819e-13d4f5e28913"
            }
          ]
        },
        {
          "id": "c084939e-687e-4383-9428-4154b04d4749",
          "name": "describeChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeChangeSet?ChangeSetName=ChangeSetName&NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the inputs for the change set and a list of changes that AWS CloudFormation will make if you execute the change set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab1623f8-29ca-4e11-bd3b-ed604f0faa1d"
            }
          ]
        },
        {
          "id": "a4f70f79-b707-44ea-ad7e-a75dbd01ea2d",
          "name": "executeChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=ExecuteChangeSet?ChangeSetName=ChangeSetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a stack using the input information that was provided when the specified change set was created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b808039-7770-4816-851e-f99e9467a934"
            }
          ]
        },
        {
          "id": "283c40f3-6b9b-4565-9e2b-d95efd20979c",
          "name": "listChangeSets",
          "request": {
            "url": "http://example.com/api/?Action=ListChangeSets?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the ID and status of each active change set for a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "834ebaff-e74a-4d1a-836d-1d99a44e9972"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "a9b70ec5-d158-44a5-91a0-4387bd275ba5",
          "name": "describeAccountLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountLimits?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves your account's AWS CloudFormation limits, such as the maximum number of stacks that you can create in your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbfb9e60-0714-4553-85e9-3ed8b8953947"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Events",
      "item": [
        {
          "id": "c89b0b7b-0ed7-4c6e-af8d-23b1c3ea42d0",
          "name": "describeStackEvents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackEvents?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all stack related events for a specified stack in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b03ada85-8346-4149-9139-fbc9e2e713e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Resources",
      "item": [
        {
          "id": "6d05ed5d-ca32-493b-afb0-c5a6e81ec1eb",
          "name": "describeStackResource",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackResource?LogicalResourceId=LogicalResourceId&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the specified resource in the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad91b613-a104-4b2b-a10b-d5ee95cb859e"
            }
          ]
        },
        {
          "id": "e8dc3c2b-c609-4a46-90fd-d62fcd0f8709",
          "name": "describeStackResources",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackResources?LogicalResourceId=LogicalResourceId&PhysicalResourceId=PhysicalResourceId&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns AWS resource descriptions for running and deleted stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "754358d4-90ab-485d-a440-6d5c6c8d4e7d"
            }
          ]
        },
        {
          "id": "a17a82fe-f7fc-4b4d-839f-7d4b2b47028d",
          "name": "listStackResources",
          "request": {
            "url": "http://example.com/api/?Action=ListStackResources?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns descriptions of all resources of the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dea89f5-3d69-491b-ae0d-98c40d2746fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Template Cost",
      "item": [
        {
          "id": "182da034-3480-4672-a753-767e65bf9aa1",
          "name": "estimateTemplateCost",
          "request": {
            "url": "http://example.com/api/?Action=EstimateTemplateCost?Parameters.member.N=Parameters.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the estimated monthly cost of a template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df9a5303-5f5f-49ce-a60e-c86444c038b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Policies",
      "item": [
        {
          "id": "1cd96739-0704-4b70-874b-9b50df2cac47",
          "name": "getStackPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetStackPolicy?StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the stack policy for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96bdc2be-5da8-4085-bd22-6a0fe411d73e"
            }
          ]
        }
      ]
    },
    {
      "name": "Templates",
      "item": [
        {
          "id": "fc43eb93-8a1a-485c-b3ef-14572fbeba93",
          "name": "getTemplate",
          "request": {
            "url": "http://example.com/api/?Action=GetTemplate?ChangeSetName=ChangeSetName&StackName=StackName&TemplateStage=TemplateStage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the template body for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8aa69c0-ce60-4342-925b-5eeb8f815b99"
            }
          ]
        },
        {
          "id": "b7824f21-7698-469a-af9f-865f7b3688ab",
          "name": "getTemplateSummary",
          "request": {
            "url": "http://example.com/api/?Action=GetTemplateSummary?StackName=StackName&TemplateBody=TemplateBody&TemplateURL=TemplateURL",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a new or existing template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9801bfae-6717-41b7-9d75-f5ec15729cd8"
            }
          ]
        }
      ]
    },
    {
      "name": "Exports",
      "item": [
        {
          "id": "737ff62b-0d47-4d9e-a77d-dcbab4e54879",
          "name": "listExports",
          "request": {
            "url": "http://example.com/api/?Action=ListExports?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all exported output values in the account and region in which you call this action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "014d0621-ce7c-4f4d-b0fb-98121a04ef9a"
            }
          ]
        }
      ]
    },
    {
      "name": "Imports",
      "item": [
        {
          "id": "989c8436-da6d-42a5-8457-c5964182c1c6",
          "name": "listImports",
          "request": {
            "url": "http://example.com/api/?Action=ListImports?ExportName=ExportName&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all stacks that are importing an exported output value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e7c350a-df03-4837-9bcb-40f5f090fd59"
            }
          ]
        }
      ]
    }
  ]
}