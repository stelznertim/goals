Short term goal 28.02.2022 until estimated 4.03.2022
Acquire knowledge about APIs and get comfortable with Endpoints
Aimed improvement: APIs(Why an API, Routing for provided endpoints, Accessibility, RESTfulness,http/https verbs, openAPI)
TU → CK

### Why an API?

To have a communication channel of a set of functionalities between two parties. Only the information/functionality necessary is made visible and transmitted.
Therefore it helps in encapsulation as well as security. Also all functionality needed for the data transmit is in a single place so its easier to maintain and adjust accordingly.
There are structure guidelines for good API Service building. InVision uses RESTful Design and the OpenApi specification.

### Endpoint

Is the touching point for the API and basically just an URL. Thats also the point where the consumer should get all necessary information from.

### REST

Transfers a state of the requester to the endpoint in JSON format.
Needs for an API to be acknowledged as an RESTful API:

- Client Server Architecture,
- requests through http,
- stateless communication(no client information is stored, each request is separated and unconnected),
- layered system(Middleware),
- uniform interface --> information is transferred in standard form (contract)

### Contract

The contract is an agreement on how the data should be structured in order to use the API --> Documentation structure.
We set this structure in a yaml file with the OpenApi specification. It includes endpoint urls, actions, request and response bodys, params and their data types , property requirements.
Contracts help in starting the implementation on the consumer side before the api is finished

### GET

Request data from a server. With an attached ID you get only the specified object and without an ID you get an collection of objects.

### POST

Will on each request create a new resource entry. Should always be used for create operations instead of PUT.

### PUT

Will create a new resource entry if the resource is not there yet otherwise it will update the entire resource. Should be used to update not create if possible. Idempotent.

### PATCH

Used if you want to only update part of a resource, otherwise use put for full update of a resource.

### DELETE

Deletes requested resource. Idempotent.

### Access
