{
  "info": {
    "name": "AWS CloudFormation API Create Change Set",
    "_postman_id": "893e696b-5999-415b-a929-a3abd7a7d379",
    "description": "Creates a list of changes for a stack.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "576bf595-c633-41db-a368-6420b60239ba",
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
              "id": "76e40a0f-65ed-466f-a9e0-5702489c38ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "d80a12c2-ea83-48f5-b329-fd3873cc07b3",
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
              "id": "4bdc156c-3f94-4971-8524-b898e6b3f341"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Sets",
      "item": [
        {
          "id": "4deef5a6-1f4d-424d-aac2-33eeba2a2068",
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
              "id": "b6840821-b43b-4e77-b107-49bad2dcde1c"
            }
          ]
        }
      ]
    }
  ]
}