{
  "info": {
    "name": "AWS CloudFormation API Delete Change Set",
    "_postman_id": "16cabfae-9be8-423c-990a-155b5063ff3d",
    "description": "Deletes the specified change set.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "b2997afc-82d2-41d3-97ba-5ef71eba55c7",
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
              "id": "80e7dd8a-05f5-48bb-bec8-a4e279fd6033"
            }
          ]
        },
        {
          "id": "359da17e-df0d-47be-8a1b-9ecb3dd6faa0",
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
              "id": "79149bfa-d3e7-46c4-b910-2009c6eb7481"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "4c1ad067-3fcd-426e-8c6b-b02f9b9b7f5b",
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
              "id": "fc72cdbf-e2a6-429c-bfbb-6f98fe5879e3"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Sets",
      "item": [
        {
          "id": "addbe95e-28a9-4e11-b921-9776a25bf72f",
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
              "id": "5d5ac93f-b871-451f-b5ea-2d559f5515fb"
            }
          ]
        },
        {
          "id": "8c58aa73-64ac-4320-90f4-1ff72bb93aeb",
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
              "id": "9bab4157-7f51-4534-988d-20e6b6a69748"
            }
          ]
        }
      ]
    }
  ]
}