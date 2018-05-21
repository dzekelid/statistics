{
  "info": {
    "name": "Azure Data Lake Analytics API Job Get Statistics",
    "_postman_id": "792a233a-ce3c-4adf-8412-bfee88b0d1bd",
    "description": "Gets statistics of the specified job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Catalog Table Statistics",
      "item": [
        {
          "id": "0ec8c675-b45c-4136-ba2b-d629a1e432dc",
          "name": "Catalog_ListTableStatistics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "catalog/usql/databases/:databaseName/schemas/:schemaName/tables/:tableName/statistics"
              ],
              "query": [
                {
                  "key": "$count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$orderby",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$select",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "databaseName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "schemaName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tableName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the list of table statistics from the Data Lake Analytics catalog."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44b518ce-9d44-4396-b4d3-14e5fa9cf73b"
            }
          ]
        }
      ]
    },
    {
      "name": "Job Statistics",
      "item": [
        {
          "id": "632a6993-9301-4a4c-a2e0-def94a2078e0",
          "name": "Job_GetStatistics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "Jobs/:jobIdentity/GetStatistics"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "jobIdentity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets statistics of the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa0fd600-25bc-4544-af15-85db186d6624"
            }
          ]
        }
      ]
    }
  ]
}