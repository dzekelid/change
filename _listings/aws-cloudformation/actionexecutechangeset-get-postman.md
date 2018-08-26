{
  "info": {
    "name": "AWS CloudFormation API Execute Change Set",
    "_postman_id": "aba6c40e-4d85-41fd-a5c2-8c9084cc8597",
    "description": "Updates a stack using the input information that was provided when the specified change set was created.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "30dac65a-305e-4669-a868-6b788aa71238",
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
              "id": "178f568b-b4ea-45d9-9671-57f4aa316a45"
            }
          ]
        },
        {
          "id": "9376eda0-f2c7-4be8-84ed-aa37a91aeb78",
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
              "id": "1ecea14e-af07-44c5-a8b3-06bb79b6c43b"
            }
          ]
        },
        {
          "id": "bb9a55e6-7e12-471e-83a7-5add15764adc",
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
              "id": "8d67abd1-65f7-4c34-980e-e3565fc127cf"
            }
          ]
        },
        {
          "id": "416cf98c-3fca-4b53-a4f9-074ea70140f3",
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
              "id": "64d12606-0842-4298-b4ac-5dc1ad78cc4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "fdff1b24-f4b5-46b4-bae0-21e9dd1278d4",
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
              "id": "e5acc3ea-992c-41f4-875e-8e7ec2945122"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Sets",
      "item": [
        {
          "id": "ceba053e-a078-4730-b5df-62f49f747e7e",
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
              "id": "93e8316f-f183-402c-bd48-1f104c602aec"
            }
          ]
        },
        {
          "id": "806566be-f052-4105-be0c-349e618f5bc6",
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
              "id": "091abf8e-38e4-4667-8736-2df5f25ec062"
            }
          ]
        },
        {
          "id": "447c65e6-8da5-4f54-a641-b49e6d007691",
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
              "id": "c1420865-e235-43c0-b5ea-49ceb11da77f"
            }
          ]
        },
        {
          "id": "abec9784-bca2-4663-a781-87f25b4cd384",
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
              "id": "c5670eeb-47b6-4bb9-9785-f2b624c24028"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "66e24ce7-3658-4e2a-b045-af44fd2640b7",
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
              "id": "717d9400-c495-4156-b046-fa3e5c38d6ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Events",
      "item": [
        {
          "id": "8564062a-8730-4664-a34c-377837510df4",
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
              "id": "36fa57a2-b268-4dda-91d3-96b9d73c1cb1"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Resources",
      "item": [
        {
          "id": "c707433a-e261-406b-b8e0-c36bc899277f",
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
              "id": "a5e2277e-b3cb-4e43-afb1-1180882fd6ff"
            }
          ]
        },
        {
          "id": "82ce7b82-0277-43eb-848e-6d2a6d7137a9",
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
              "id": "d6e22eb1-dc68-48ed-9968-50cb48557a81"
            }
          ]
        }
      ]
    },
    {
      "name": "Template Cost",
      "item": [
        {
          "id": "ff30fe53-654b-4450-bfe6-121e388d7c07",
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
              "id": "a15fb9ad-0af2-40a8-a442-6b2f32119e19"
            }
          ]
        }
      ]
    }
  ]
}