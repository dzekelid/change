{
  "info": {
    "name": "Google Drive Get Start Page Token Changes",
    "_postman_id": "d4d9e1b3-84ca-4b69-b76b-61d0b454fd7e",
    "description": "Gets the starting pageToken for listing future changes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "About",
      "item": [
        {
          "id": "263e33c2-fa37-4c46-ac55-74d79101636b",
          "name": "drive.about.get",
          "request": {
            "url": "http://www.googleapis.com/drive/v3/about",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the user, the user's Drive, and system capabilities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5250d84-9fc0-4c08-bd71-8ffdb0f0dd9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "540c9368-fcf7-4d39-b696-681b2aa433d1",
          "name": "drive.changes.list",
          "request": {
            "url": "http://www.googleapis.com/drive/v3/changes?includeCorpusRemovals=%7B%7D&includeRemoved=%7B%7D&includeTeamDriveItems=%7B%7D&pageSize=%7B%7D&pageToken=%7B%7D&restrictToMyDrive=%7B%7D&spaces=%7B%7D&supportsTeamDrives=%7B%7D&teamDriveId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the changes for a user or Team Drive."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfa206c0-39f7-4607-bcfe-f23f227a5a76"
            }
          ]
        },
        {
          "id": "db7d4b60-1c71-4fdd-ae29-fb590839b5e4",
          "name": "drive.changes.getStartPageToken",
          "request": {
            "url": "http://www.googleapis.com/drive/v3/changes/startPageToken?supportsTeamDrives=%7B%7D&teamDriveId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the starting pageToken for listing future changes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68e502b3-2e89-4667-8009-716f893d6da1"
            }
          ]
        }
      ]
    }
  ]
}