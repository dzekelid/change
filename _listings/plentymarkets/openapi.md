---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/plugin_sets/{setId}/plugins/{pluginId}:
    put:
      summary: Change a plugin's 'active' status for a set.
      description: Change a plugin's 'active' status for a set..
      operationId: putRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-put
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Plugins
      - Active
      - Statusa
      - Set
---