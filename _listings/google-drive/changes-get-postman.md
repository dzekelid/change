{
  "info": {
    "name": "Google Drive Get Changes",
    "_postman_id": "030e6812-6d40-45c9-a2e7-a864f0963af4",
    "description": "Lists the changes for a user or Team Drive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "About",
      "item": [
        {
          "id": "340c67a6-57f2-41dc-85cb-aa632153663c",
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
              "id": "293e706f-c6c2-4ac9-8bb3-730412ef654f"
            }
          ]
        }
      ]
    },
    {
      "name": "Change",
      "item": [
        {
          "id": "9aa5530b-03cf-4912-a686-45294477d5bf",
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
              "id": "6097150e-b5a4-4ae2-8469-2488cdf1b4df"
            }
          ]
        }
      ]
    }
  ]
}