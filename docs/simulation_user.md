
### /s2s/simulation_user/add

#### POST
##### Summary:

Add simulation user

##### Description:

Create new Simulation user

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationUserEntity | body |  | Yes | [SimulationUserEntity](#simulationuserentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with Simulation user object |
| 400 | Bad request |
| 500 | Internal Server error |

### /s2s/simulation_user/update

#### PUT
##### Summary:

Update simulation user

##### Description:

Update simulation user

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationUserEntity | body |  | Yes | [SimulationUserEntity](#simulationuserentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with updated simulation user object |
| 400 | Bad request |
| 500 | Internal Server error |

### /s2s/simulation_user

#### GET
##### Summary:

Get all entities

##### Description:

Get all entities

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_user/{id}

#### GET
##### Summary:

Get an entity by id

##### Description:

Get an entity by id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with matching object |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_user/softdelete/{id}

#### DELETE
##### Summary:

Soft delete an entity by id

##### Description:

Soft delete an entity by id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | Entity id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with deleted object |
| 404 | Not found error with custom message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_user/delete/{id}

#### DELETE
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |

