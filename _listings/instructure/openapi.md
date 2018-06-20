---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Courses API
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/quizzes/quiz_id/statistics:
    get:
      summary: Fetching the latest quiz statistics
      description: Fetching the latest quiz statistics.
      operationId: fetching-the-latest-quiz-statistics
      x-api-path-slug: coursescourse-idquizzesquiz-idstatistics-get
      parameters:
      - in: query
        name: all_versions
        description: Whether the statistics report should include all submissions
          attempts
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Statistics
---