{
  "info": {
    "name": "Amazon EC2 Container Service API Submit Task State Change",
    "_postman_id": "d7e134cf-e460-4cc9-a827-8ac9ca9385a1",
    "description": "This action is only used by the Amazon EC2 Container Service agent, and it is not intended for use outside of the agent.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Task Definitions",
      "item": [
        {
          "id": "c8a69b42-36e2-49b3-bb5f-d15c6c75eccb",
          "name": "deregisterTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskDefinition?taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters the specified task definition by family and revision."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ea09573-cf2c-4576-b825-0f2fc9122d45"
            }
          ]
        },
        {
          "id": "18db4cb4-1f19-49ea-acda-84e9ff7b4f94",
          "name": "describeTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTaskDefinition?taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a task definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "457a8898-ad5f-4f3d-9ea1-bb99cba86a5e"
            }
          ]
        },
        {
          "id": "1fc131fb-cd50-4b20-b834-29b3a3eddce1",
          "name": "listTaskDefinitions",
          "request": {
            "url": "http://example.com/api/?Action=ListTaskDefinitions?familyPrefix=familyPrefix&maxResults=maxResults&nextToken=nextToken&sort=sort&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of task definitions that are registered to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81236c8c-185a-45d6-bd6a-69eafea5cab7"
            }
          ]
        },
        {
          "id": "1e2e9f67-8c5d-4117-8d2a-1e9375a4eed2",
          "name": "registerTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=RegisterTaskDefinition?containerDefinitions=containerDefinitions&family=family&networkMode=networkMode&placementConstraints=placementConstraints&taskRoleArn=taskRoleArn&volumes=volumes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a new task definition from the supplied family and\n                containerDefinitions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53bd69ad-83a1-4f70-87ea-74bb9738a95c"
            }
          ]
        }
      ]
    },
    {
      "name": "Tasks",
      "item": [
        {
          "id": "5d79b231-2aa6-4a30-bd0d-19eeb012c415",
          "name": "describeTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTasks?cluster=cluster&tasks=tasks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a specified task or tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca7cb433-12d8-4edd-9e1b-3a0ca38417ce"
            }
          ]
        },
        {
          "id": "1cc6c8c4-5fdb-4f1a-a8cf-54e4664ecf20",
          "name": "listTasks",
          "request": {
            "url": "http://example.com/api/?Action=ListTasks?cluster=cluster&containerInstance=containerInstance&desiredStatus=desiredStatus&family=family&maxResults=maxResults&nextToken=nextToken&serviceName=serviceName&startedBy=startedBy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tasks for a specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "713fe52c-9ab4-429b-8661-6e10395b256a"
            }
          ]
        },
        {
          "id": "fa0afade-b0c8-4588-83bf-5d42f1817918",
          "name": "runTask",
          "request": {
            "url": "http://example.com/api/?Action=RunTask?cluster=cluster&count=count&group=group&overrides=overrides&placementConstraints=placementConstraints&placementStrategy=placementStrategy&startedBy=startedBy&taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a new task using the specified task definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54679b97-0119-4c4d-ac5d-067566042df4"
            }
          ]
        },
        {
          "id": "82a2e9ab-2e64-4d5e-99ab-ff094b3655fc",
          "name": "startTask",
          "request": {
            "url": "http://example.com/api/?Action=StartTask?cluster=cluster&containerInstances=containerInstances&group=group&overrides=overrides&startedBy=startedBy&taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a new task from the specified task definition on the specified container\n            instance or instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51f72eb7-480f-4741-a4ec-3d1c7e65ae72"
            }
          ]
        },
        {
          "id": "95c58610-58c8-4bfe-9993-dffccfd8d4ad",
          "name": "stopTask",
          "request": {
            "url": "http://example.com/api/?Action=StopTask?cluster=cluster&reason=reason&task=task",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops a running task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a4394f9-a7c7-46ac-987b-3d0cf5a80fe6"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Definition Families",
      "item": [
        {
          "id": "70fd5ea3-e295-4c5f-bb07-ae0641cbbbaf",
          "name": "listTaskDefinitionFamilies",
          "request": {
            "url": "http://example.com/api/?Action=ListTaskDefinitionFamilies?familyPrefix=familyPrefix&maxResults=maxResults&nextToken=nextToken&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of task definition families that are registered to your account\n            (which may include task definition families that no longer have any ACTIVE\n            task definition revisions)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4167ac68-21bc-4002-8400-dc96c8bf1db6"
            }
          ]
        }
      ]
    },
    {
      "name": "Task State Change",
      "item": [
        {
          "id": "986a0d0e-d0f0-4fb8-9b1f-c21fb0a2c66b",
          "name": "submitTaskStateChange",
          "request": {
            "url": "http://example.com/api/?Action=SubmitTaskStateChange",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This action is only used by the Amazon EC2 Container Service agent, and it is not intended for use outside of the agent."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8fc2c26-7851-430a-8524-8b3f8d530fdb"
            }
          ]
        }
      ]
    }
  ]
}