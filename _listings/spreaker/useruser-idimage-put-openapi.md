---
swagger: "2.0"
x-collection-name: Spreaker
x-complete: 0
info:
  title: Spreaker API Change User Profile Image
  version: v1
  description: Change User Profile Image
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /episode/<episode_id>/image:
    put:
      summary: Change Episode Image
      description: Change Episode Image
      operationId: putEpisode<episode>Image
      x-api-path-slug: episodeepisode-idimage-put
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      - in: query
        name: image_id
        description: The id of the image to set to the episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - Episode
      - Image
  /user/{user_id}/image:
    put:
      summary: Change User Profile Image
      description: Change User Profile Image
      operationId: putUserUserImage
      x-api-path-slug: useruser-idimage-put
      parameters:
      - in: query
        name: image_id
        description: The id of the image to set to the user profile
      - in: path
        name: user_id
        description: The unique user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - User
      - Profile
      - Image
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---