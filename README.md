# Batiklens-API

# Description
Using Express.js and Node.js to build an API is chosen due to the combination of high performance, lightweight structure, extensive community support, robust middleware, clear routing system, good scalability, easy implementation of RESTful principles, and built-in support for JSON data exchange. These advantages make Node.js and Express.js a superior choice for API development projects, enabling developers to achieve optimal performance and development efficiency.

# How to Use
- `npm install`

# Endpoint Route

- ### Add Batik

  - URL Route:
    `/api/addBatik/` 

  - Method:
    POST

  - Request Body:

    - `name` as `string`
    - `description` as `string`
    - `imageUrl` as `string`

  - Response:
    - Status : 200
      ```
      {
          "message": 'Batik added successfully',
          "id": batikRef.id 
      }
      ```
    - Status : 400
      ```
      {
          "error": 'All fields are required'
      }
      ```
    - Status : 500
      ```
      {
          "error": 'Internal Server Error'
      }
      ```
  

- ### Get All Batiks

  - URL Route:
    `/api/allBatiks`

  - Method:
    GET

  - Response:
      ```
      {
      "id": "batik ID",
      "name": "name batik",
      "description": "batik description",
      "imageUrl": "https://batik-image.com"
      }
      ```
- ### Get Batik By ID

  - URL Route:
    `/api/batik/:id` 

  - Method:
    GET

  - Response:
      ```
      {
          "name": 'batik name',
          "description": 'batik description',
          "imageUrl": 'https://batik-image'
      }
      ```
