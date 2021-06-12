# Marvel Characters API
The objective of this project is to create a backend web-service (REST API) that returns information about Marvel characters. The project is split into several phases. 

## Phase 1
Create two REST HTTP endpoints for retrieving character information:

#### GET /characters
This endpoint should return a complete list of all of the characters that the backend service has.

#### GET /characters/:character-id 
This endpoint should return a single character with the corrosponding `character-id`.

## Phase 2
Add the ability to filter the results that are returned from the `GET /characters` endpoint that was created in Phase 1. 

## Phase 3
Create an endpoint that allows clients to create new characters. 

#### POST /characters
This endpoint accepts a JSON body payload and stores the character information in the service so that it can be retrieved later.

## Phase 4
Create two endpoints that modify and delete characters, respectively.

#### PUT /characters/:character-id
This endpoint accepts a JSON body payload and updates the service's data store with the new character information that was sent to the endpoint.

#### DELETE /characters/:character-id
This endpoint instructs the web-service to delete the character record in the underlying data store. 

## Phase 5
Connect the web service to a persistent data store (e.g. SQL database, document store, KV store, JSON file, CSV, etc.) that will persist the character information across service restarts. 

---

## API Interface
### Responses
Responses from the web service should be JSON. Use appropriate [HTTP status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) for each kind of response.

### Requests
Requests should accept JSON for data payloads.

--- 

## Data

You can use the data in `marvel_characters_info.csv` (credit to [dannielr on Kaggle](https://www.kaggle.com/dannielr/marvel-superheroes?select=marvel_characters_info.csv)) for sample data that may be returned by the API.