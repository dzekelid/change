{
  "info": {
    "name": "Plentymarkets Change a plugin's 'active' status for a set.",
    "_postman_id": "bf887e8c-0cdc-4423-b29f-0e399ffe386f",
    "description": "Change a plugin's 'active' status for a set..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Change",
      "item": [
        {
          "id": "58adcb34-8d56-4777-a72d-2a3566931c7e",
          "name": "putRestPluginSetsSetPluginsPlugin",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/plugin_sets/:setId/plugins/:pluginId"
              ],
              "variable": [
                {
                  "id": "pluginId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "setId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Change a plugin's 'active' status for a set.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d31ff60d-a194-46e4-8f90-ae1bd82a972e"
            }
          ]
        }
      ]
    }
  ]
}