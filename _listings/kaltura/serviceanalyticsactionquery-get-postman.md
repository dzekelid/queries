{
  "info": {
    "name": "Kaltura VPaaS Get Service Analytics Action Query",
    "_postman_id": "a3bb5a72-ca0b-46e6-af85-e79f48b21d7b",
    "description": "report query action allows to get a analytics data for specific query dimensions, metrics and filters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "840a86ba-57a3-49a3-ba8d-d89286a107f2",
          "name": "analytics.query",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/analytics/action/query?filter[dimensions]=%7B%7D&filter[filters]=%7B%7D&filter[from_time]=%7B%7D&filter[metrics]=%7B%7D&filter[orderBy]=%7B%7D&filter[to_time]=%7B%7D&filter[utcOffset]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "report query action allows to get a analytics data for specific query dimensions, metrics and filters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "498fc9e2-6a11-4a9e-be91-458586fed9d3"
            }
          ]
        }
      ]
    }
  ]
}