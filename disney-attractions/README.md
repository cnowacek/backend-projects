# Disney Attractions API
The objective of this project is to create a backend web-service (REST API) that returns information about Disney theme park attractions. The project is split into several phases. 

## Phase 1
Create two REST HTTP endpoints for retrieving attraction information:

#### GET /attractions
This endpoint should return a complete list of all of the attractions that the backend service has.

#### GET /attractions/:attraction-id 
This endpoint should return a single attraction with the corrosponding `attraction-id`.

## Phase 2
Add the ability to filter the results that are returned from the `GET /attractions` endpoint that was created in Phase 1. 

## Phase 3
Create an endpoint that allows clients to create new attractions. 

#### POST /attractions
This endpoint accepts a JSON body payload and stores the attraction information in the service so that it can be retrieved later.

## Phase 4
Create two endpoints that modify and delete attractions, respectively.

#### PUT /attractions/:attraction-id
This endpoint accepts a JSON body payload and updates the service's data store with the new attraction information that was sent to the endpoint.

#### DELETE /attractions/:attraction-id
This endpoint instructs the web-service to delete the attraction record in the underlying data store. 

## Phase 5
Connect the web service to a persistent data store (e.g. SQL database, document store, KV store, JSON file, CSV, etc.) that will persist the attraction information across service restarts. 

---

## API Interface
### Responses
Responses from the web service should be JSON. Use appropriate [HTTP status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) for each kind of response.

### Requests
Requests should accept JSON for data payloads.

--- 

## Data

You can use the data in `WDW_Ride_Data_DW.xlsx` (credit to [Lynne Passanisi on data.world](https://data.world/lynne588/walt-disney-world-ride-data)) for sample data that may be returned by the API.